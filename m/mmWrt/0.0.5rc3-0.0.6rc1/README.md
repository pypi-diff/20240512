# Comparing `tmp/mmWrt-0.0.5rc3-py3-none-any.whl.zip` & `tmp/mmWrt-0.0.6rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 12172 bytes, number of entries: 11
+Zip file size: 17932 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat     2937 b- defN 24-May-12 16:58 mmWrt/Plots.py
 -rw-rw-rw-  2.0 fat       10 b- defN 23-Jan-14 13:58 mmWrt/PointCloud.py
--rw-rw-rw-  2.0 fat     9972 b- defN 23-Dec-28 09:25 mmWrt/RadarSignalProcessing.py
--rw-rw-rw-  2.0 fat     6152 b- defN 23-Dec-28 09:25 mmWrt/Raytracing.py
--rw-rw-rw-  2.0 fat     7424 b- defN 23-Dec-28 09:25 mmWrt/Scene.py
--rw-rw-rw-  2.0 fat       29 b- defN 23-Dec-28 09:29 mmWrt/__init__.py
+-rw-rw-rw-  2.0 fat    12352 b- defN 24-May-12 16:58 mmWrt/RadarSignalProcessing.py
+-rw-rw-rw-  2.0 fat    12633 b- defN 24-May-12 16:58 mmWrt/Raytracing.py
+-rw-rw-rw-  2.0 fat    14315 b- defN 24-May-12 16:58 mmWrt/Scene.py
+-rw-rw-rw-  2.0 fat       29 b- defN 24-May-12 17:00 mmWrt/__init__.py
 -rw-rw-rw-  2.0 fat     1329 b- defN 23-Jan-07 11:55 mmWrt/fmcw.py
--rw-rw-rw-  2.0 fat     1095 b- defN 23-Dec-28 12:13 mmWrt-0.0.5rc3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3963 b- defN 23-Dec-28 12:13 mmWrt-0.0.5rc3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Dec-28 12:13 mmWrt-0.0.5rc3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Dec-28 12:13 mmWrt-0.0.5rc3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      840 b- defN 23-Dec-28 12:13 mmWrt-0.0.5rc3.dist-info/RECORD
-11 files, 30912 bytes uncompressed, 10762 bytes compressed:  65.2%
+-rw-rw-rw-  2.0 fat     1095 b- defN 24-May-12 17:02 mmWrt-0.0.6rc1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5293 b- defN 24-May-12 17:02 mmWrt-0.0.6rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 17:02 mmWrt-0.0.6rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-12 17:02 mmWrt-0.0.6rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      914 b- defN 24-May-12 17:02 mmWrt-0.0.6rc1.dist-info/RECORD
+12 files, 51005 bytes uncompressed, 16418 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: mmWrt/Plots.py
+Comment: 
+
 Filename: mmWrt/PointCloud.py
 Comment: 
 
 Filename: mmWrt/RadarSignalProcessing.py
 Comment: 
 
 Filename: mmWrt/Raytracing.py
@@ -12,23 +15,23 @@
 
 Filename: mmWrt/__init__.py
 Comment: 
 
 Filename: mmWrt/fmcw.py
 Comment: 
 
-Filename: mmWrt-0.0.5rc3.dist-info/LICENSE
+Filename: mmWrt-0.0.6rc1.dist-info/LICENSE
 Comment: 
 
-Filename: mmWrt-0.0.5rc3.dist-info/METADATA
+Filename: mmWrt-0.0.6rc1.dist-info/METADATA
 Comment: 
 
-Filename: mmWrt-0.0.5rc3.dist-info/WHEEL
+Filename: mmWrt-0.0.6rc1.dist-info/WHEEL
 Comment: 
 
-Filename: mmWrt-0.0.5rc3.dist-info/top_level.txt
+Filename: mmWrt-0.0.6rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: mmWrt-0.0.5rc3.dist-info/RECORD
+Filename: mmWrt-0.0.6rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mmWrt/RadarSignalProcessing.py

```diff
@@ -1,10 +1,9 @@
 from numpy import array, sqrt, log2, log, pi
 from scipy.fft import fft
-from numpy import complex_ as complex
 from numpy import angle
 
 
 def error(targets_synthetics, targets_f):
     """ Computes the error in the targets position estimation
 
     Parameters
@@ -35,14 +34,15 @@
             targets_i.pop(idx0)
             if len(targets_i) == 0:
                 break
 
     # if less targets found than inserted
     # add the remaining ones to the error
     for t in targets_i:
+        # d = t.distance()
         total_error += t.distance()
 
     # FIXME: add here code in case missing targets or
     # excessive targets in the found target list
 
     return total_error
 
@@ -165,70 +165,156 @@
                 mag_max = mag_r[idx]
                 idx_max = idx
         idx_peaks.append(idx_max)
         cluster = []
     return idx_peaks
 
 
-def range_fft(baseband, chirp_index=0, fft_window=None, fft_padding=0):
+def range_resolution(v, B):
+    """ Range resolution is c/2B
+
+    Parameters
+    ----------
+    v: float
+        celerity of light in medium
+    B: float
+        Bandwidth of signal sampled (often simplified as chirped)
+
+    Returns
+    -------
+    delta_R: float
+        Range Resolution
+    """
+    delta_R = v/2/B
+    return delta_R
+
+
+def if2d(radar):
+    """ ratio from IF frequency to distance
+    !!! important
+
+        the ratio is 1/2 of the d2f as the IF frequency results from the wave
+        traveling to the target and back. Whereas if2d gives the distance
+        between the radar and the scatterer which is 1/2 the distance
+        travelled by the radar EM wave.
+
+    Parameters
+    ----------
+    radar: object
+        a radar object
+
+    Returns
+    --------
+    f2d: float
+        ratio between frequency and distance for given radar
+        settings
+
+    Usage
+    -----
+    f2d = if2d(radar)
+    # assuming f_if is an IF frequency
+    # then d will be the distsance to the target
+    d = f2d * f_if
+    """
+
+    f2d = radar.v/2/radar.slope
+    return f2d
+
+
+def range_fft(baseband, chirp_index=0,
+              fft_window=None, fft_padding=0,
+              full_FFT=False,
+              debug=False):
     """ scipy FFT wrapper with windowing and padding options
 
     Parameters
     ----------
     baseband: numpy array
         the IF ADC signals data matrix
     chirp_index: int
         index of the chirp in the data matrix
     fft_window: str
         FFT windowing names supported by scipy get_window
     fft_padding: int
         if 0 - no padding
         if -1: padding to next level of power of 2
         other values: padding to those values
+    full_FFT: bool
+        if True returns the full FFT, else only 0..d_max_unambiguous
+    debug: bool
+        if True logs debug information on console
 
     Returns
     -------
     Range_FFT: tuple
         Distances: np array
         abs_FT: np array
 
     Raises
     ------
     ValueError
         when fft_padding has a value < -1
     """
     if chirp_index == 0:
         # v0.1.1: adc = baseband['adc_cube'][0][0][0]
-        adc = baseband['adc_cube'][0, chirp_index, 0, 0, :]
+        frame_idx = 0
+        rx_idx = 0
+        tx_idx = 0
+        adc = baseband['adc_cube'][frame_idx, chirp_index, tx_idx, rx_idx, :]
     else:
         raise ValueError("chirp index value not supported yet")
 
     if fft_padding == -1:
+        if debug:
+            print("padding FFT to next **2")
         fft_length = 2**int(log2(len(adc)) + 1)
     elif fft_padding == 0:
+        if debug:
+            print(f"no FFT padding, using len: {len(adc)}")
         fft_length = len(adc)
-    elif fft_padding < 0:
+    elif fft_padding < -1:
         raise ValueError(f"Unsupported fft padding value with : {fft_padding}")
     else:
+        if debug:
+            print(f"padding up to len: {fft_padding} as opposed " +
+                  f"to adc len of: {len(adc)}")
         fft_length = fft_padding
 
     if fft_window is None:
+        if debug:
+            print("FFT without windowing")
         FT = fft(adc, n=fft_length)
     else:
+        if debug:
+            print(f"FFT windowing, using: {fft_window}")
         from scipy.signal import get_window
         w = get_window(fft_window, len(adc))
         FT = fft(adc * w, n=fft_length)
-    if baseband["datatype"] == complex:
-        pass
+
+    delta_R = range_resolution(baseband["v"], baseband["bw"])
+    # Because R_MAX is real, FS-MAX > FIF_MAX * 2
+    delta_R_FFT = (baseband["fs"]/2)*baseband["v"] \
+        / ((len(FT)) * baseband["slope"] * 2)
+    Distances = [i * delta_R_FFT for i in range(len(FT)//2)] + \
+        [-i * delta_R_FFT for i in range(len(FT)//2, len(FT))]
+
+    if debug:
+        print(f"Range Resolution: {delta_R:.2g}, based on chirping")
+        print(f"Range resolution based on sampling:{delta_R_FFT:.2g}")
+
+    if full_FFT:
+        if debug:
+            print("FULL FFT")
     else:
         # return half of FFT for real bb signal
+        if debug:
+            print("returning only half of FFT (non ambiguous ranges/volicity)")
         FT = FT[:len(FT)//2]
-    Distances = [i * baseband["fs"] / adc.shape[0] *
-                 baseband["v"]/2/baseband["slope"]
-                 for i in range(len(FT))]
+        Distances = Distances[:len(Distances)//2]
+
     Range_FFT = (Distances, FT)
     return Range_FFT
 
 
 def __quinnsecond__(FT, k):
     """ Provide frequency estimator via Quinn's second estimate
```

## mmWrt/Raytracing.py

```diff
@@ -1,14 +1,14 @@
-from numpy import arctan2, arange, cos, exp, pi, sqrt, zeros
+from numpy import arctan2, arange, exp, pi, sqrt, zeros, real
 from numpy import float32  # alternatives: float16, float64
 from numpy import complex_ as complex
 
 
 def BB_IF(f0_min, slope, T, antenna_tx, antenna_rx, target,
-          medium, datatype=float32, radar_equation=False):
+          medium, datatype=float32, radar_equation=False, debug=False):
     """ This function implements the mathematical IF defined in latex as
     y_{IF} = cos(2 \\pi [f_0\\delta + s * \\delta * t - s* \\delta^2])
     into following python code
     y_IF = cos (2*pi*(f_0 * delta + slope * delta * T + slope * delta**2))
 
     Parameters
     ----------
@@ -26,38 +26,55 @@
         instance of Target()
     medium : Medium
         instance of Medium
     datatype: type
         either float16, 32, 64 or complex128
     radar_equation: bool
         if True adds Radar Equation contribution to IF values
+    debug: bool
+        if True displays debug information
     Returns
     -------
     YIF : ndarray
         vector containing the IF values
     """
+    # while T is the absolute time
+    # Tc is the relative time to begining of chirp (and of the ramp)
+    Tc = T-T[0]
     tx_x, tx_y, tx_z = antenna_tx.xyz
     rx_x, rx_y, rx_z = antenna_rx.xyz
-    t_x, t_y, t_z = target.pos(T[0])
+    t_x, t_y, t_z = target.pos_t(T[0])
     v = medium.v
     L = medium.L
     distance = sqrt((tx_x - t_x)**2 + (tx_y - t_y)**2 + (tx_z - t_z)**2)
     distance += sqrt((rx_x - t_x)**2 + (rx_y - t_y)**2 + (rx_z - t_z)**2)
-    azimuth_rx = arctan2(rx_x-t_x, rx_y-t_y)
-    azimuth_tx = arctan2(tx_x-t_x, tx_y-t_y)
-    elevation_rx = arctan2(rx_y-t_y, rx_z-t_z)
-    elevation_tx = arctan2(tx_y-t_y, tx_z-t_z)
+    if debug:
+        print(f"distance: {distance:.2g}")
+    # note delta_time is d/v because d is already there and back
+    # (usually 2*d in text books)
     delta = distance / v
+    if debug:
+        print(f"delta t: {delta:.2g}")
+    # compute fif_max for upper layer to ensure Nyquist
     fif_max = 2*slope*distance/v
-    if datatype == complex:
-        YIF = exp(2 * pi * 1j *
-                  (f0_min * delta + slope * delta * T + slope * delta**2))
-    else:
-        YIF = cos(2 * pi *
-                  (f0_min * delta + slope * delta * T + slope * delta**2))
+    if debug:
+        print("fi_if", fif_max)
+    # FIXME: replace here T by Time inside chirp (different from system time)
+    YIF = exp(2 * pi * 1j *
+              (f0_min * delta + 2 * slope * delta * Tc - slope * delta**2))
+    # if debug:
+    #    print("YIF", YIF)
+    if not datatype == complex:
+        YIF = real(YIF)
+    # if datatype == complex:
+    #    YIF = exp(2 * pi * 1j *
+    #              (f0_min * delta + slope * delta * T + slope * delta**2))
+    # else:
+    #    YIF = cos(2 * pi *
+    #              (f0_min * delta + slope * delta * T + slope * delta**2))
     # here bring in the radar equation
     # target_type and RCS
     # most targets will have 1/R*4, corner reflector as 1/R**2
     # and antenna radiation patterns in azimuth, elevation
     # and frequency response
     # f0 being the center frequency of the chirp
     # f0 = f0_min + slope*(T[-1]-T[0])/2
@@ -68,30 +85,40 @@
     # Prx = Ptarget * L
     # else
     # Prx = Ptarget * 1/(4*pi*distance**2) * L
     # Where L = Medium Losses during propagation *
     #       fluctuation Losses (often modeled w/ Swerling models)
     # Prx_e = Prx * AW (where AW is effective area RX antenna)
     # Prx_c = Prx_c * Gr(azimuth, elevation, f0)
-    f0 = f0_min + slope*(T[-1]-T[0])/2
-    YIF = YIF * antenna_tx.gain(azimuth_tx, elevation_tx, f0) \
-        * antenna_rx.gain(azimuth_rx, elevation_rx, f0)
     if radar_equation:
+        # FIXME: add here that with physic samples should be `0`
+        # for T<distance/v
+        # because of ToF no mixing possible...
+        azimuth_rx = arctan2(rx_x-t_x, rx_y-t_y)
+        azimuth_tx = arctan2(tx_x-t_x, tx_y-t_y)
+        elevation_rx = arctan2(rx_y-t_y, rx_z-t_z)
+        elevation_tx = arctan2(tx_y-t_y, tx_z-t_z)
+
+        f0 = f0_min + slope*(T[-1]-T[0])/2
+        YIF = YIF * antenna_tx.gain(azimuth_tx, elevation_tx, f0) \
+            * antenna_rx.gain(azimuth_rx, elevation_rx, f0)
+
         YIF = YIF * target.rcs(f0)
         if target.target_type == "corner_reflector":
             YIF = YIF / distance**2
         else:
             YIF = YIF / distance**4
         YIF = YIF * 10**(L*distance)
     IF = (YIF, fif_max)
     return IF
 
 
 def rt_points(radar, targets, radar_equation=False,
-              datatype=float32, debug=False):
+              datatype=float32, debug=False,
+              raytracing_opt={"compute": True}):
     """ raytracing with points
 
     Parameters
     ----------
     radar: Radar
         instance of Radar
     targets: List[Target]
@@ -99,14 +126,19 @@
     radar_equation: bool
         if True includes the radar equation when computing the IF signal
         else ignores radar equation
     datatype: Type
         type of data to be generate by rt: float16, float32, ... or complex
     debug: bool
         if True increases level of print messages seen
+    raytracing_opt: dict
+        compute: bool
+            if True computes raytracing (use False for radar statistics tuning)
+        T_start: float
+            time offset to start simulation
 
     Returns
     -------
     baseband: dict
         dictonnary with adc values and other parameters used later in analysis
 
     Raises
@@ -117,44 +149,164 @@
     n_frames = radar.frames_count
     # n_chirps is the # chirps each TX antenna sends per frame
     n_chirps = radar.chirps_count
     n_tx = len(radar.tx_antennas)
     n_rx = len(radar.rx_antennas)
     n_adc = radar.n_adc
     ts = 1/radar.fs
+    bw = radar.bw
     adc_cube = zeros((n_frames, n_chirps, n_tx, n_rx, n_adc)).astype(datatype)
+    times = zeros((n_frames, n_chirps, n_tx, n_rx, n_adc))
     f0_min = radar.f0_min
     slope = radar.slope
-    T = arange(0, n_adc*ts, ts)
+    T = arange(0, n_adc, 1)
+    # T is the absolute time across the simulation
+    T = T*ts
+    assert len(T) == n_adc
+    if "T_start" in raytracing_opt:
+        T += raytracing_opt["T_start"]
+    if "logger" not in raytracing_opt:
+        raytracing_opt["logger"] = "logger"
+
+    v = radar.medium.v
+    Tc = bw/slope
+    if n_chirps > 1:
+        try:
+            assert Tc > n_adc*ts
+        except Exception as ex:
+            log_msg = f"{str(ex)} for Tc: {Tc:.2g} vs NA*TS: {n_adc*ts: .2g}"
+        try:
+            assert radar.t_inter_chirp > Tc
+        except Exception as ex:
+            log_msg = f"{str(ex)} for Tc: {Tc:.2g} vs " + \
+                f"T_interchip: {radar.t_inter_chirp: .2g}"
+            raise ValueError(log_msg)
 
-    for chirp_i in range(n_chirps):
-        for tx_i in range(n_tx):
-            T[:] += radar.t_interchirp
-            for rx_i in range(n_rx):
-                YIF = zeros(n_adc).astype(datatype)
-                for target in targets:
-                    YIFi, fif_max = BB_IF(f0_min, slope, T,
-                                          radar.tx_antennas[tx_i],
-                                          radar.rx_antennas[rx_i],
-                                          target,
-                                          radar.medium,
-                                          radar_equation=radar_equation,
-                                          datatype=datatype)
-                    # ensure Nyquist is respected
-                    try:
-                        assert fif_max * 2 <= radar.fs
-                    except AssertionError:
-                        if debug:
-                            print(f"failed Nyquist for target: {tx_i}" +
-                                  f"fif_max is: {fif_max} " +
-                                  f"radar ADC fs is: {radar.fs}")
-                        raise ValueError("Nyquist will always prevail")
-                    YIF += YIFi
-                adc_cube[0, chirp_i, tx_i, rx_i, :] = YIF
+    if n_frames > 1:
+        try:
+            assert radar.t_inter_frame > (radar.t_inter_chirp*n_chirps)
+        except Exception as ex:
+            log_msg = f"{str(ex)} for TF: {radar.t_inter_frame:.2g} " +\
+                f"vs NC*T_interchip: {radar.t_inter_chirp*n_chirps: .2g}"
+            raise ValueError(log_msg)
 
-    baseband = {"adc_cube": adc_cube, "frames_count": n_frames,
+    baseband = {"adc_cube": adc_cube,
+                "frames_count": n_frames,
                 "chirps_count": radar.chirps_count,
-                "t_interchirp": radar.t_interchirp, "n_tx": n_tx,
-                "n_rx": n_rx, "datatype": datatype,
-                "f0_min": f0_min, "slope": slope, "T": T,
+                "t_inter_chirp": radar.t_inter_chirp,
+                "n_tx": n_tx,
+                "n_rx": n_rx,
+                "n_adc": n_adc,
+                "datatype": datatype,
+                "f0_min": f0_min,
+                "slope": slope,
+                "bw": bw,
+                "Tc": Tc,
+                "TFFT": n_adc*ts,
+                "T": T,
                 "fs": radar.fs, "v": radar.v}
+
+    # T_start = T[0]
+    Tc = T
+    # compute can be set to False, when only interested in chirp statistics
+    if raytracing_opt["compute"]:
+        for frame_i in range(n_frames):
+            for chirp_i in range(n_chirps):
+                for tx_i in range(n_tx):
+                    for rx_i in range(n_rx):
+                        YIF = zeros(n_adc).astype(datatype)
+                        T = Tc + (radar.t_inter_frame*frame_i) + \
+                            (radar.t_inter_chirp*(chirp_i+1))
+                        for target in targets:
+                            YIFi, fif_max = BB_IF(f0_min, slope, T,
+                                                  radar.tx_antennas[tx_i],
+                                                  radar.rx_antennas[rx_i],
+                                                  target,
+                                                  radar.medium,
+                                                  radar_equation=radar_equation,  # noqa E501
+                                                  datatype=datatype,
+                                                  debug=debug)
+                            # ensure Nyquist is respected
+                            try:
+                                assert fif_max * 2 <= radar.fs
+                            except AssertionError:
+                                log_msg = "Nyquist will always prevail: " +\
+                                    f"fs:{radar.fs:.2g} vs f_if:{fif_max:.2g}"
+                                if debug:
+                                    print(f"!! Nyquist for target: {target}" +
+                                          f"fif_max is: {fif_max} " +
+                                          f"radar ADC fs is: {radar.fs}")
+                                    raise ValueError(log_msg)
+                            YIF += YIFi
+                        adc_cube[frame_i, chirp_i, tx_i, rx_i, :] = YIF
+                        times[frame_i, chirp_i, tx_i, rx_i, :] = T
+                        YIF, YIFi = None, None
+
+        baseband["adc_cube"] = adc_cube
+        # T_fin = ((Tc +t_inter_chirp * NC) + t_inter_frame)*n_frames+ Tc
+        baseband["times"] = times
+        baseband["T_fin"] = T[-1]
+
+    if debug:
+        print("Generic observations about the simulation")
+        print(f"Compute: {raytracing_opt['compute']}")
+        print(f"Radar freq: {radar.tx_antennas[0].f_min_GHz} GHz")
+        print("ADC samples #", n_adc)
+        range_resolution = radar.medium.v/(2*radar.transmitter.bw)
+        print("range resolution", range_resolution)
+
+        if "Dres_min" in raytracing_opt:
+            print("Range resolution target vs actual",
+                  raytracing_opt["Dres_min"], range_resolution)
+        else:
+            print("Range resolution", range_resolution)
+        Tc = bw/slope
+        print("Tc", Tc)
+        print("T[-1]", T[-1])
+        print("ts", ts)
+        print("N adc per chirp", n_adc)
+        print("t_interchirp", radar.t_inter_chirp)
+        frame_time = n_adc*ts + radar.t_inter_chirp
+        print("frame timing:", frame_time)
+        print("simulation time", frame_time * n_frames)
+
+        print("Dmax", v*Tc/2)
+        print("Dmax as function fs", radar.fs*v/2/slope)
+        radar_lambda = radar.medium.v/radar.tx_antennas[0].f_min_GHz/1e9
+        print(f"radar lambda: {radar_lambda}")
+        if radar.t_inter_chirp > 0 and radar.chirps_count > 0:
+            vmax = radar_lambda/4/radar.t_inter_chirp
+            print(f"vmax :{vmax}")
+            vref_IF = radar_lambda/2/radar.chirps_count/Tc
+            print(f"speed resolution (within a frame of N chirps): {vref_IF}")
+        else:
+            print("no speed info as only one chirp transmitted")
+        # vres = lambda / 2 / N / Tc
+        # vres_intrachirp =
+        # vres_interframe =
+        # vres_intraframe = radar_lambda/2/Tc
+        # print(f"speed resolution intra-frame: {vres_intraframe}")
+
+        print("---- TARGETS ---")
+        for idx, target in enumerate(targets):
+            x0, y0, z0 = target.pos_t()
+            x1, y1, z1 = target.pos_t(t=T[-1])
+            d0 = sqrt(x0**2 + y0**2 + z0**2)
+            d1 = sqrt(x1**2+y1**2+z1**2)
+
+            distance_covered = sqrt((x0-x1)**2 + (y0-y1)**2 + (z0-z1)**2)
+            target_if = 2*slope*target.distance()/radar.medium.v
+
+            print(f"IF frequency for target[{idx}] is {target_if}, "
+                  f"which is {target_if/radar.fs:.2g} of fs")
+
+            if distance_covered > range_resolution:
+                print("!!!!!! target[{idx}] covers more than one range: "
+                      f"{distance_covered} vs {range_resolution}")
+                print(f"initial position: {d0} and final position: {d1}")
+            else:
+                print(f"----- target[{idx}] covers less than one range: " +
+                      f"{distance_covered} < {range_resolution} range res.")
+            print(f"Range index: from {d0//range_resolution} "
+                  f"to {d1//range_resolution}")
+            print(f"End of simulation time: {T[-1]}")
     return baseband
```

## mmWrt/Scene.py

```diff
@@ -1,45 +1,106 @@
 # from .Transmitter import Transmitter as Transmitter
 # from .Receiver import Receiver as Receiver
 # from .Radar import Radar as Radar
 
-from numpy import log2, pi, sqrt, zeros
+from numpy import all, log2, pi, sqrt, zeros
 
 
 class Target():
-    def __init__(self, x=0, y=0, z=0,
-                 vx=lambda t: 0, vy=lambda t: 0, vz=lambda t: 0,
+    def __init__(self, x=0.0, y=0.0, z=0.0,
+                 xt=None, yt=None, zt=None,
                  rcs_f=lambda f: 1,
                  target_type="point"):
+        """ Initializes a target, ease of use vs simplicity at definition
+
+        Parameters
+        ----------
+        x: float
+            x-coordinate
+        y: float
+            y-coordinate
+        z: float
+            z-coordindate
+        xt: lambda
+            x-coordinate in time
+        yt: lamda
+            y-coordinate in time
+        zt: lambda
+            z-coordinate in time
+        rcs_f: lambda
+            lambda of rcs as function of frequency
+        target_type: str
+            point or volume
+
+        Raises
+        ------
+        ValueError
+            when definition of x(0) is not x and x is different than 0
+
+        Usage:
+        ------
+        define a target at (x,y,z)=(0,0,0)
+        > target = Target()
+        define a target at (x,y,z)=(10,0,0)
+        > target = Target(10)
+        define a target with a position in time x(t) = 10 + 10*t
+        > target = Target(xt= lambda t: 10 + 10*t)
+        """
         self.x = x
         self.y = y
         self.z = z
-        self.vx = vx
-        self.vy = vy
-        self.vz = vz
+
+        if xt is not None:
+            if x != 0:
+                assert x == xt(0)
+            else:
+                self.x = xt(0)
+            self.xt = xt
+        else:
+            self.xt = lambda t: x
+
+        if yt is not None:
+            if y != 0:
+                assert y == yt(0)
+            else:
+                self.y = yt(0)
+            self.yt = yt
+        else:
+            self.yt = lambda t: y
+
+        if zt is not None:
+            if z != 0:
+                assert z == zt(0)
+            else:
+                self.z = zt(0)
+            self.zt = zt
+        else:
+            self.zt = lambda t: z
+
         self.rcs_f = rcs_f
         self.target_type = target_type
 
     def speed(self):
+        raise ValueError("speed not in usage anymore")
         v = (self.vx, self.vy, self.vz)
         return v
 
     def distance(self, target=None, t=0):
-        x0, y0, z0 = self.pos(t)
+        x0, y0, z0 = self.pos_t(t)
         if target is None:
             x1, y1, z1 = 0, 0, 0
         else:
-            x1, y1, z1 = target.pos(t)
+            x1, y1, z1 = target.pos_t(t)
         dist = sqrt((x0-x1)**2 + (y0-y1)**2 + (z0-z1)**2)
         return dist
 
-    def pos(self, t=0):
-        x0, y0, z0 = self.x, self.y, self.z
-        vx, vy, vz = self.speed()
-        position_t = (x0+vx(t), y0+vy(t), z0+vz(t))
+    def pos_t(self, t=0):
+        # x0, y0, z0 = self.x, self.y, self.z
+        xt, yt, zt = self.xt(t), self.yt(t), self.zt(t)
+        position_t = (xt, yt, zt)
         return position_t
 
     def __str__(self):
         return f"x0:{self.x}, y0:{self.y}, z0:{self.z}"
 
     def rcs(self, f):
         return self.rcs_f(f)
@@ -87,17 +148,26 @@
             frequency in Hertz
 
         Returns
         -------
         gain_dB: float
             gain in dB
 
+        Raises
+        ------
+        ValueError
+            if freq is too low
         """
         freq_GHz = freq / 1e9
-        assert freq_GHz > self.f_min_GHz
+        try:
+            assert freq_GHz > self.f_min_GHz
+        except Exception as ex:
+            print(f"{str(ex)}freq_GHz, self.f_min_GHz",
+                  freq_GHz, self.f_min_GHz)
+            raise ValueError("freq")
         assert freq_GHz < self.f_max_GHz
         idx = int((freq_GHz-self.f_min_GHz)*self.look_up)
         gain_db10 = self.freq_gains_db10[idx]
         return gain_db10
 
     def gain(self, azimuth, elevation, freq):
         """ computes total antenna gain over elevation, aziumth and frequency
@@ -112,113 +182,232 @@
             frequency at which antenna gain needs to be calculated
 
         Returns
         -------
         overall_gain: float
             antenna gain at freq and given direction
         """
-        azimuth_deg = int((azimuth+pi)*180/pi)
-        elevation_deg = int((elevation+pi)*180/pi)
+        azimuth_deg = int((azimuth+pi)*180/pi) % 360
+        elevation_deg = int((elevation+pi)*180/pi) % 360
         gain_angle_db = self.angle_gains_db10[azimuth_deg, elevation_deg]
         gain_freq = self.freq_gain_db10(freq)
         overall_gain = 10**gain_angle_db * 10**gain_freq
         return overall_gain
 
 
 class Receiver():
     def __init__(self,
                  fs=4e2,
                  antennas=(Antenna(),),
                  max_adc_buffer_size=1024,
                  max_fs=25e6,
+                 n_adc=0,
                  config=None,
                  debug=False):
         self.fs = fs
         self.antennas = antennas
         self.max_adc_buffer_size = max_adc_buffer_size
+        self.n_adc = n_adc
         try:
             assert fs < max_fs
         except AssertionError:
             if debug:
                 print(f"fs:{fs} > max_fs: {max_fs}")
             raise ValueError("ADC sampling value must stay below max_fs")
         return
 
 
 class Transmitter():
     def __init__(self,
                  f0_min=60e9,
-                 slope=250e6,
+                 slope=None,
+                 slope_MHz_us=None,
                  bw=4e9,
                  antennas=(Antenna(),),
-                 t_interchirp=0,
+                 t_inter_chirp=0.0,
                  chirps_count=1,
+                 t_inter_frame=0.0,
                  frames_count=1,
                  conf=None):
         """Transmitter class models a radar transmitter
 
         Parameters
         ----------
         f0_min: float
             start frequency of the chirp
-        slope: float
+        slope: Optional[float]
             the slope of the linearly growing chirp frequency
+        slope_MHz_us: Optional[float]
+            mutually exclusive with slope being slope parameter
+            slope in MHz/us: a 4 GHz in 16 us is 250 MHz/us.
         bw: float
             bandwidth of the chirp (i.e. fmax-fmin)
         antennas: List[Antenna]
             transmitter Antennas instances
-        t_interchirp: float
+        t_inter_chirp: float
             time increment between two TX antennas sending a chirp
         chirps_count: int
             The # chirps each TX antenna sends per frame
+        t_inter_frame: float
+            time increment between end of last chirp in frame N-1 and
+            first chirp in frame N (offset on top of
+            t_inter_chirp). If t_interframe==0, then there will be a
+            single t_inter_chirp offset.
         frames_count: int
             The number of iterations where each TX antennas send chirps_count
         conf: dict
             additional optional parameters (reserved for future usage)
         """
+        if slope is None and slope_MHz_us is None:
+            slope_MHz_us = 250
+        if slope is not None and slope_MHz_us is not None:
+            assert ValueError("only slope or slope_MHz_us can be specified")
+        if slope is None:
+            slope = slope_MHz_us * 1e12  # type: ignore
+        assert slope > 1e8
         self.f0_min = f0_min
         self.slope = slope
-        self.t_interchirp = t_interchirp
+        self.t_inter_chirp = t_inter_chirp
         self.chirps_count = chirps_count
         self.antennas = antennas
+        if t_inter_frame == 0:
+            self.t_inter_frame = t_inter_chirp
+        else:
+            assert t_inter_frame >= t_inter_chirp
+            self.t_inter_frame = t_inter_frame
         self.frames_count = frames_count
         self.bw = bw
         return
 
 
 class Medium:
-    def __init__(self, v=3e8, L=0):
-        # v default to c=3e8 speed of light in void
-        # L defaults to 0 dB/m losses in medium
+    def __init__(self, v=3e8, L=0, name="void"):
+        """ initialises the medium where demo runs
+
+        Parameters
+        ----------
+        v: float
+            speed of light in the given medium, defaults to 3e8 for void
+        L: float
+            attenuation in dB/m in given medium, defaults to 0 for void
+        name: str
+            name of the given medium, defaults to void
+        """
         self.v = v
         self.L = L
+        self.name = name
+        if name == "void":
+            # Ensuring consistency with physics
+            assert v == 3e8
+            assert L == 0
 
 
 class Radar:
     def __init__(self, transmitter=Transmitter(), receiver=Receiver(),
                  medium=Medium(), adc_po2=False, debug=False):
+        """ Defines a Radar instance from Transmitter class, Receiver class,
+        Medium class
+        and allows overriding the number of adc samples.
+
+        Parameters
+        ----------
+        transmitter: Transmitter()
+            definition of the transmitter chain used
+        receiver: Receiver()
+            definition of the receiver chain used
+        medium: Medium()
+            definition of the medium used (currently only uniform medium)
+        adc_po2: bool
+            if true sets number of ADC to next power of 2 from current value
+        debug: bool
+            if True: prints error message
+            else: raises exception
+
+        Raises
+        ------
+        ValueError
+            if ADC buffer exceeds maximum buffer size
+        """
         self.transmitter = transmitter
         self.rx_antennas = receiver.antennas
         self.tx_antennas = transmitter.antennas
+
         self.frames_count = transmitter.frames_count
+        self.n_adc = receiver.n_adc
         self.fs = receiver.fs
-        self.n_adc = int(transmitter.bw / transmitter.slope * receiver.fs)
+        self.bw = transmitter.bw
+        if self.n_adc == 0:
+            self.n_adc = int(transmitter.bw * receiver.fs / transmitter.slope)
+            if self.n_adc == 0:
+                log_msg = f"nadc updated to 0: {transmitter.bw:.2g}" +\
+                    f"{receiver.fs:.2g}= {transmitter.bw*receiver.fs:.2g}" +\
+                    f" /  {transmitter.slope:.2g}"
+                # , transmitter.bw, receiver.fs, transmitter.slope
+                print(log_msg)
+            if debug:
+                print("updating NADC from 0 to:", self.n_adc)
+        t_fft = receiver.n_adc / receiver.fs
+        t_chirp = transmitter.bw / transmitter.slope
+
+        bw_adc = self.n_adc*transmitter.slope/receiver.fs
+        if bw_adc < 0.8 * transmitter.bw:
+            print(f"! BW ADC: {bw_adc:.2g} << chirp: {transmitter.bw:.2g}")
+        if debug:
+            print(f"Bandwidth in chirp: {transmitter.bw:.2g}")
+            print(f"Bandwidth in ADC buffers: {bw_adc:.2g}")
+        if self.n_adc < 8:
+            print("!!!! ADC # low", self.n_adc)
+            print("BW", transmitter.bw)
+            print("BW GHz", transmitter.bw/1e9)
+            print("K", transmitter.slope)
+            print("K/1e12", transmitter.slope/1e12)
+            print("TC", transmitter.bw / transmitter.slope)
+            print("N_ADC", transmitter.bw / transmitter.slope * receiver.fs)
+
         if adc_po2:
             self.n_adc = 2 ** int(log2(self.n_adc))
             n_adc = self.n_adc
             assert n_adc / receiver.fs * transmitter.slope < transmitter.bw
         self.f0_min = transmitter.f0_min
         self.slope = transmitter.slope
-        self.t_interchirp = transmitter.t_interchirp
+        self.t_inter_chirp = transmitter.t_inter_chirp
         self.chirps_count = transmitter.chirps_count
+        self.t_inter_frame = transmitter.t_inter_frame
+        self.frames_count = transmitter.frames_count
         self.v = medium.v
         self.medium = medium
-        self.range_bin = self.fs * self.v / 2 / self.slope / self.n_adc
-        # f*c/2/k
-        self.f2d = medium.v * receiver.fs / 2 / transmitter.slope / self.n_adc
+        self.bw = transmitter.bw
+        # FIXME: moves this to simulation level
+        # __range_bin: deprecated as relies on c for compute
+        # __c = 3e8
+        # self.range_bin_deprec = receiver.fs*__c/2/self.slope/self.n_adc
+
+        if all(self.rx_antennas[0].angle_gains_db10 == 0):
+            for idx, _ in enumerate(self.rx_antennas):
+                self.rx_antennas[idx].f_min_GHz = self.f0_min/1e9
+                self.rx_antennas[idx].f_max_GHz = (self.f0_min + self.bw)/1e9
+            if debug:
+                print("rx fmin", self.rx_antennas[idx].f_min_GHz)
+                print("rx fmax", self.rx_antennas[idx].f_max_GHz)
+
+        if all(self.tx_antennas[0].angle_gains_db10 == 0):
+            for idx, _ in enumerate(self.rx_antennas):
+                self.tx_antennas[idx].f_min_GHz = self.f0_min/1e9
+                self.tx_antennas[idx].f_max_GHz = (self.f0_min + self.bw)/1e9
+            if debug:
+                print("tx fmin", self.tx_antennas[idx].f_min_GHz)
+                print("tx fmax", self.tx_antennas[idx].f_max_GHz)
+        try:
+            assert t_fft <= t_chirp
+        except AssertionError:
+            if debug:
+                print(f"T_FFT: {t_fft:.2g}")
+                print(f"T_C: {t_chirp:.2g}")
+            raise ValueError("TC should be longer than T_FFT")
+
         try:
             assert self.n_adc < receiver.max_adc_buffer_size
         except AssertionError:
             if debug:
                 print(f"buffer size: {self.n_adc} > " +
                       f"vs max buffer size: {receiver.max_adc_buffer_size}" +
                       f"ratio: {self.n_adc/receiver.max_adc_buffer_size}")
```

## mmWrt/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.5-pre.3"
+__version__ = "0.0.6-pre.1"
```

## Comparing `mmWrt-0.0.5rc3.dist-info/LICENSE` & `mmWrt-0.0.6rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mmWrt-0.0.5rc3.dist-info/METADATA` & `mmWrt-0.0.6rc1.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmWrt
-Version: 0.0.5rc3
+Version: 0.0.6rc1
 Summary: minimal raytracing code example for MIMO FMCW radar
 Home-page: https://github.com/matt-chv/mmWrt
 Author: matt-chv
 Author-email: contact@matthieuchevrier.com
 License: LICENSE
 Project-URL: Bug Tracker, https://github.com/matt-chv/mmWrt/issues
 Keywords: radar MIMO FMCW raytracing
@@ -27,23 +27,25 @@
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: semver
 Provides-Extra: dev
 Requires-Dist: coverage ; extra == 'dev'
 Requires-Dist: darglint ; extra == 'dev'
 Requires-Dist: flake8 ; extra == 'dev'
+Requires-Dist: jupyter ; extra == 'dev'
 Requires-Dist: myst-parser ; extra == 'dev'
 Requires-Dist: nbsphinx ; extra == 'dev'
 Requires-Dist: pyroma ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: recommonmark ; extra == 'dev'
 Requires-Dist: sphinx ; extra == 'dev'
 Requires-Dist: sphinx-markdown-builder ; extra == 'dev'
 Requires-Dist: sphinx-rtd-theme ; extra == 'dev'
 Requires-Dist: tox ; extra == 'dev'
+Requires-Dist: twine ; extra == 'dev'
 Requires-Dist: wheel ; extra == 'dev'
 
 # mmWrt
 
 minimal raytracing for MIMO FMCW radar systems.
 
 Intended usage:
@@ -63,14 +65,26 @@
 v0.0.4:
 
     * adding frequency estimator
     * added speed processing
     * added support for radar equation (RCS, distance, ...)
     * antenna gains in azimumth, elevation and freq
 
+v0.0.5:
+
+    * moved dependancies from requirements to setup.py
+    * added extras [dev] for developpers (and documentation and read the docs)
+    * moved version checking from setup.py to test_basic.py
+    * added readthedocs.yaml
+
+v0.0.6:
+
+    * added micro-doppler
+    * added non-regression on .ipynb in docs/ folder
+
 ### NEXT ()
 
     * 2D (AoA)
     * 2D FFT: range+velocity, range+AoA
     * 2D peak grouping (by velocity sign)
     * 3D position error compute
     * 3D targets (at least spheres)
@@ -134,18 +148,47 @@
 
 9. release to pypi-test
 
 > python setup.py bdist_wheel
 
 > twine upload -r testpypi dist\*
 
-10. update on read_the_docs
-
+10. check updates on read_the_docs
 
+> push to git to trigger readthedocs build:
+> git push
+> navigate to https://readthedocs.org/projects/mmwrt/builds/
+> ensure build is successful
 
 11. check on Google Colab
 (Google Colab requires py3.8 as off 2023-Jan-15)
 
+11.a. if testing release-candidate need to spell out or will install latest stable version
+
+```
+!python -m pip install -i https://test.pypi.org/simple/ mmWrt==0.0.5rc3
+from mmWrt import __version__
+print(__version__)
+```
+
+11.b seems extras cannot be imported from versions, so `pip install mmWrt=0.0.5rc3[dev]` or `pip install mmWrt==0.0.5[dev]` does not work. Need to upgrade to full version to test dev.
+
+```
+!python -m pip install -i https://test.pypi.org/simple/ mmWrt[dev]
+from mmWrt import __version__
+print(__version__)
+```
+
 12. release on pypi
 > twine upload -r pypi dist\*
 
+13. check on colab that pypi package works:
+
+>!python -m pip install mmWrt
+from mmWrt import __version__
+print(__version__)
+
+13.b. then check dev extras install works
+
+>!python -m pip install mmWrt[dev]
+
```

