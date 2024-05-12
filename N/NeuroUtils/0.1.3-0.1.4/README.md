# Comparing `tmp/NeuroUtils-0.1.3-py3-none-any.whl.zip` & `tmp/NeuroUtils-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 16619 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat    38839 b- defN 24-May-08 17:37 NeuroUtils/Architectures.py
--rw-rw-rw-  2.0 fat    21193 b- defN 24-May-10 18:42 NeuroUtils/Core.py
--rw-rw-rw-  2.0 fat    22147 b- defN 24-May-08 17:37 NeuroUtils/ML_assets.py
+Zip file size: 17233 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat    25630 b- defN 24-May-12 15:47 NeuroUtils/Architectures.py
+-rw-rw-rw-  2.0 fat    23725 b- defN 24-May-12 15:04 NeuroUtils/Core.py
+-rw-rw-rw-  2.0 fat    24791 b- defN 24-May-12 10:29 NeuroUtils/ML_assets.py
 -rw-rw-rw-  2.0 fat       50 b- defN 24-May-10 18:38 NeuroUtils/__init__.py
--rw-rw-rw-  2.0 fat      571 b- defN 24-May-10 21:27 NeuroUtils-0.1.3.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2078 b- defN 24-May-10 21:27 NeuroUtils-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-10 21:27 NeuroUtils-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-10 21:27 NeuroUtils-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      723 b- defN 24-May-10 21:27 NeuroUtils-0.1.3.dist-info/RECORD
-9 files, 85704 bytes uncompressed, 15377 bytes compressed:  82.1%
+-rw-rw-rw-  2.0 fat      571 b- defN 24-May-12 16:17 NeuroUtils-0.1.4.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2078 b- defN 24-May-12 16:17 NeuroUtils-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 16:17 NeuroUtils-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-12 16:17 NeuroUtils-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      723 b- defN 24-May-12 16:17 NeuroUtils-0.1.4.dist-info/RECORD
+9 files, 77671 bytes uncompressed, 15991 bytes compressed:  79.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: NeuroUtils/ML_assets.py
 Comment: 
 
 Filename: NeuroUtils/__init__.py
 Comment: 
 
-Filename: NeuroUtils-0.1.3.dist-info/LICENSE.txt
+Filename: NeuroUtils-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: NeuroUtils-0.1.3.dist-info/METADATA
+Filename: NeuroUtils-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: NeuroUtils-0.1.3.dist-info/WHEEL
+Filename: NeuroUtils-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: NeuroUtils-0.1.3.dist-info/top_level.txt
+Filename: NeuroUtils-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: NeuroUtils-0.1.3.dist-info/RECORD
+Filename: NeuroUtils-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## NeuroUtils/Architectures.py

```diff
@@ -118,145 +118,18 @@
         outputs = tf.keras.layers.Dense(n_classes, activation='softmax')(e0)
         # Define the model
         model = tf.keras.Model(inputs=inputs, outputs=outputs)
         
         #Return model
         return model
 
-    @staticmethod
-    def AnimalNet_v32(shape , n_classes):
-        img_H , img_W , channels = shape
-        #Functions of network:
-            
-        def Swish(x):
-            return x * tf.nn.sigmoid(x)    
-            
-            
-        def cnn_block(input_layer , expand_filters , squeeze_filters = None ,kernel_size = 3, block_layers=3):
-            if squeeze_filters is None:
-                squeeze_filters = expand_filters //4
-               
-            x = input_layer
-            for i in range(block_layers):
-                x_origin = x
-
-                x = tf.keras.layers.Conv2D(expand_filters, (1, 1), padding='same')(x)
-                x = tf.keras.layers.BatchNormalization()(x)
-                x = Swish(x)
-                    
-                
-                x = tf.keras.layers.DepthwiseConv2D((kernel_size,kernel_size), padding = 'same')(x)
-                x = tf.keras.layers.BatchNormalization()(x)
-                x = Swish(x)
-                
-                x = tf.keras.layers.Conv2D(squeeze_filters , (1,1), padding = 'same')(x)
-                x = tf.keras.layers.BatchNormalization()(x)
-
-
-                
-                x = tf.keras.layers.concatenate([x , x_origin])
-                x = tf.keras.layers.SpatialDropout2D(0.1)(x)
-                #x = tf.keras.layers.Add()([x , x_origin])
-            
-            if i >= block_layers-1:
-                # Ensure spatial dimensions match before concatenation
-                #input_layer = tf.keras.layers.Conv2D(filters //2, (1, 1), padding='same')(input_layer)            
-                x_merged = tf.keras.layers.concatenate([x , input_layer]) 
-                
-                x_merged = tf.keras.layers.Conv2D(expand_filters, (1, 1), padding='same')(x_merged)
-                x_merged = tf.keras.layers.BatchNormalization()(x_merged)
-                x_merged = Swish(x_merged)
-                
-                x_merged = tf.keras.layers.DepthwiseConv2D((kernel_size,kernel_size), padding = 'same')(x_merged)
-                x_merged = tf.keras.layers.BatchNormalization()(x_merged)
-                x_merged = Swish(x_merged)
-
-                x_merged = tf.keras.layers.Conv2D(squeeze_filters, (1, 1), padding='same')(x_merged)
-                x_merged = tf.keras.layers.BatchNormalization()(x_merged)
-                x_merged = Swish(x_merged)
-                
-                x_merged = tf.keras.layers.SpatialDropout2D(0.1)(x_merged)
-            
-            return x
-        
-
-
-        #Inputs
-        inputs = tf.keras.layers.Input((img_H, img_W, channels))
-        #########################################################
-        #########################################################
-        
-        p0 = tf.keras.layers.Conv2D(48,(5,5) , padding = 'same')(inputs)
-        p0 = tf.keras.layers.BatchNormalization()(p0)
-        p0 = Swish(p0)
-        
-        
-        
-        
-        
-        
-        d1 = cnn_block(p0 , 48  , kernel_size = 3 , block_layers = 3)
-        
-        d2 = cnn_block(d1,64  , kernel_size = 3 , block_layers = 5)
-        
-        d3 = cnn_block(d2,96  , kernel_size = 3 , block_layers = 5)
-        d3 = tf.keras.layers.MaxPooling2D((2,2))(d3)
-        
-        d4 = cnn_block(d3,192  , kernel_size = 3 , block_layers = 3)
-        
-        d5 = cnn_block(d4 , 256  , kernel_size = 3 , block_layers = 3)
-        d5 = tf.keras.layers.MaxPooling2D((2,2))(d5)
-        
-        d6 = cnn_block(d5 , 384  , kernel_size = 3 , block_layers = 4)
 
 
-        
-        e0 = tf.keras.layers.Conv2D(filters=64, kernel_size=(3, 3), strides=(4, 4), padding='same')(p0)
-      
-        e0 = tf.keras.layers.BatchNormalization()(e0)
-        e0 = Swish(e0)
-        
-        
-        e1 = tf.keras.layers.concatenate([d6,e0])
-        
-        e1 = cnn_block(e1 , 128 , 64 , kernel_size = 3 , block_layers = 2)
-
-        
-        
-        
-        e2 = tf.keras.layers.GlobalAveragePooling2D()(e1)
-        
-        e3 = tf.keras.layers.Dense(256)(e2)
-        e3 = Swish(e3)
-        e3 = tf.keras.layers.BatchNormalization()(e3)
-        e3 = tf.keras.layers.Dropout(0.2)(e3)
-        
-        e4 = tf.keras.layers.Dense(128)(e3)
-        e4 = Swish(e4)
-        e4 = tf.keras.layers.BatchNormalization()(e4)
-        e4 = tf.keras.layers.Dropout(0.5)(e4)
-        
-        e5 = tf.keras.layers.Dense(64)(e4)
-        e5 = Swish(e5)
-        e5 = tf.keras.layers.BatchNormalization()(e5)
-        e5 = tf.keras.layers.Dropout(0.4)(e5)
-        
-        
-        #########################################################
-        #########################################################
-        #Outputs 
-        outputs = tf.keras.layers.Dense(n_classes, activation='softmax')(e5)
-        # Define the model
-        model = tf.keras.Model(inputs=inputs, outputs=outputs)
-        
-        #Return model
-        return model
-    
     @staticmethod
-    def AnimalNet_v32_01(shape , n_classes):
+    def AnimalNet_v32(shape , n_classes):
         img_H , img_W , channels = shape
         #Functions of network:
             
         def Swish(x):
             return x * tf.nn.sigmoid(x)    
             
             
@@ -378,121 +251,17 @@
         # Define the model
         model = tf.keras.Model(inputs=inputs, outputs=outputs)
         
         #Return model
         return model
 
 
-    @staticmethod
-    def MobileNet_v2(shape , n_classes, alpha = 1):
-        img_H , img_W , channels = shape
-        #Functions of network:
-            
-        def Swish(x):
-            return x * tf.nn.sigmoid(x)   
-        
-        def relu6(x):
-            return min(max(0, x), 6)
-        
-        
-        def inv_residual_block(x , filters , t = 6 , s = 1 ):
-
-            squeeze = filters//t
-            
-
-            # Expansion phase: 1x1 convolution to increase channel dimensionality
-            m = tf.keras.layers.Conv2D(filters, (1, 1))(x)
-            m = tf.keras.layers.BatchNormalization()(m)
-            m = Swish(m)
-            
-            # Depthwise convolution phase
-            m = tf.keras.layers.DepthwiseConv2D((3, 3), strides=(s, s), padding='same')(m)
-            m = tf.keras.layers.BatchNormalization()(m)
-            m = Swish(m)
-            
-            # Squeeze phase: 1x1 convolution to decrease channel dimensionality
-            m = tf.keras.layers.Conv2D(squeeze, (1, 1))(m)
-            m = tf.keras.layers.BatchNormalization()(m)
-            
-            b = tf.keras.layers.Conv2D(squeeze, (1, 1))(x)
-            if s == 1:
-                final = tf.keras.layers.Add()([m,b])
-                return final
-            else:
-                return m
-        
-        def bottleneck(x , t , c , n , s):
-            for i in range(n):
-                if s >1:
-                    x = inv_residual_block(x , c , t , s)
-                    s = 1
-                else:
-                    x = inv_residual_block(x , c , t , s)
-                    
-            return x
-                    
-
-
-        inputs = tf.keras.layers.Input((img_H, img_W, channels))
-        
-        c0 = tf.keras.layers.Conv2D(32*alpha, (3,3),strides=(2,2), padding="same")(inputs)
-        
-        b1 = bottleneck(c0 , t=1 , c=int(16*alpha) , n=1 , s=1)
-        b1 = tf.keras.layers.SpatialDropout2D(0.1)(b1)
-        
-        b2 = bottleneck(b1 , t=6 , c=int(24*alpha) , n=2 , s=2)
-        b2 = tf.keras.layers.SpatialDropout2D(0.1)(b2)
-        
-        b3 = bottleneck(b2 , t=6 , c=int(32*alpha) , n=3 , s=2)
-        b3 = tf.keras.layers.SpatialDropout2D(0.1)(b3)
-        
-        b4 = bottleneck(b3 , t=6 , c=int(64*alpha) , n=4 , s=2)
-        b4 = tf.keras.layers.SpatialDropout2D(0.1)(b4)
-        
-        b5 = bottleneck(b4 , t=6 , c=int(96*alpha) , n=3 , s=1)
-        b5 = tf.keras.layers.SpatialDropout2D(0.1)(b5)
-        
-        b6 = bottleneck(b5 , t=6 , c=int(160*alpha) , n=3 , s=2)
-        b6 = tf.keras.layers.SpatialDropout2D(0.1)(b6)
-        
-        b7 = bottleneck(b6 , t=6 , c=int(320*alpha) , n=1 , s=1)
-        b7 = tf.keras.layers.SpatialDropout2D(0.1)(b7)
-        
-        c8 = tf.keras.layers.Conv2D(int(1280*alpha), (1,1), padding="same")(b7)
-        c8 = Swish(c8)
-        
-        a9 = tf.keras.layers.GlobalAveragePooling2D()(c8)
-        
-        
-        d0 = tf.keras.layers.Dense(int(256*alpha))(a9)
-        d0 = Swish(d0)
-        d0 = tf.keras.layers.BatchNormalization()(d0)
-        d0 = tf.keras.layers.Dropout(0.1)(d0)
-        
-        d0 = tf.keras.layers.Dense(int(128*alpha))(d0)
-        d0 = Swish(d0)
-        d0 = tf.keras.layers.BatchNormalization()(d0)
-        d0 = tf.keras.layers.Dropout(0.15)(d0)
-        
-        d0 = tf.keras.layers.Dense(int(64*alpha))(d0)
-        d0 = Swish(d0)
-        d0 = tf.keras.layers.BatchNormalization()(d0)
-        d0 = tf.keras.layers.Dropout(0.1)(d0)
-        
-
-        
-        
-        outputs = tf.keras.layers.Dense(n_classes, activation='softmax')(d0)
-
-        model = tf.keras.Model(inputs=[inputs], outputs=[outputs])
-        return model
-
 
     @staticmethod
-    def MobileNet_v2_corrected(shape , n_classes, alpha = 1):
+    def MobileNet_v2(shape , n_classes, alpha = 1):
         img_H , img_W , channels = shape
         #Functions of network:
             
         def Swish(x):
             return x * tf.nn.sigmoid(x)   
         
         def relu6(x):
@@ -588,14 +357,16 @@
         
         
         outputs = tf.keras.layers.Dense(n_classes, activation='softmax')(d0)
 
         model = tf.keras.Model(inputs=[inputs], outputs=[outputs])
         return model    
 
+
+
     @staticmethod
     def StupidNet(shape , n_classes):
         img_H , img_W , channels = shape
 
 
         
         inputs = tf.keras.layers.Input((img_H, img_W, channels))
@@ -665,197 +436,14 @@
 
         model = tf.keras.Model(inputs=[inputs], outputs=[outputs])
         return model
 
 
 
     @staticmethod
-    def ResNet_own(shape , n_classes):
-        img_H , img_W , channels = shape
-        
-        def Swish(x):
-            return x * tf.nn.sigmoid(x)  
-
-        
-        def res_small_block(x , f , s , drop):
-            if s>1:
-                r = tf.keras.layers.Conv2D(f , (3,3) , strides = (s,s) , padding = "same")(x)
-                r = tf.keras.layers.BatchNormalization()(r)
-                r = Swish(r)
-                
-                r = tf.keras.layers.Conv2D(f , (3,3) , strides = (1,1) , padding = "same")(r)
-                r = tf.keras.layers.BatchNormalization()(r)
-                r = Swish(r)
-                
-            else:
-                r = tf.keras.layers.Conv2D(f , (3,3) , strides = (1,1) , padding = "same")(x)
-                r = tf.keras.layers.BatchNormalization()(r)
-                r = Swish(r)
-                
-                r = tf.keras.layers.Conv2D(f , (3,3) , strides = (1,1) , padding = "same")(r)
-                r = tf.keras.layers.BatchNormalization()(r)
-                r = Swish(r)
-                
-            
-
-            
-            if s == 1:
-                r = tf.keras.layers.Add()([x,r])
-                r = tf.keras.layers.SpatialDropout2D(drop)(r)
-                return r
-            else:
-                r = tf.keras.layers.SpatialDropout2D(drop)(r)
-                return r
-            
-            
-            
-            
-        def res_main_block(x , filters , depth, strides = 1 , drop = 0.1):
-            m = x
-            for i in range(depth):
-                x = res_small_block(x , filters , strides , drop)
-                
-                if strides >1:
-                    strides = 1
-            m = tf.keras.layers.Conv2D(filters , (3,3) , strides = (2,2) , padding = "same")(m)
-            m = tf.keras.layers.concatenate([x,m])
-            m = tf.keras.layers.Conv2D(filters , (1,1) , padding = "valid")(m)
-            m = tf.keras.layers.BatchNormalization()(m)
-            m = Swish(m)
-            m = tf.keras.layers.SpatialDropout2D(drop*2)(m)
-            
-            return m
-                
-
-        #For later use of auto-scaling network by img_size
-        #count = int(math.floor(math.log(img_H / small_format, 2)))
-        
-        
-        
-        
-        
-        inputs = tf.keras.layers.Input((img_H, img_W, channels))
-        
-        
-        x = tf.keras.layers.Conv2D(64, (7,7) ,padding = "same")(inputs)
-        
-        x = res_main_block(x , 64 , 3 , strides = 2)
-        x = res_main_block(x , 128 , 4 , strides = 2)
-        x = res_main_block(x , 256 , 6 , strides = 2)
-        x = res_main_block(x , 512 , 3 , strides = 2)
-        
-        x = tf.keras.layers.GlobalAveragePooling2D()(x)
-        
-        x = tf.keras.layers.Dense(1024)(x)
-        x = tf.keras.layers.BatchNormalization()(x)
-        x = Swish(x)
-        
-
-
-            
-            
-            
-
-
-        outputs = tf.keras.layers.Dense(n_classes, activation='softmax')(x)
-
-        model = tf.keras.Model(inputs=[inputs], outputs=[outputs])
-        return model
-        
-
-    @staticmethod
-    def ResNet_50(shape , n_classes):
-        img_H , img_W , channels = shape
-        
-        def Swish(x):
-            return x * tf.nn.sigmoid(x)  
-        
-        def conv_batch_relu(x , filters , kernel_size , strides = 1):
-            x = tf.keras.layers.Conv2D(filters , kernel_size , strides , padding = "same")(x)
-            x = tf.keras.layers.BatchNormalization()(x)
-            x = Swish(x)
-            
-            return x
-
-                
-        def identity_block(tensor , filters):
-            x = conv_batch_relu(tensor , filters = filters , kernel_size = 1 , strides = 1)
-            x = conv_batch_relu(x , filters = filters , kernel_size = 3 , strides = 1)
-            
-            x = tf.keras.layers.Conv2D(filters*4 , kernel_size = 1 , strides = 1)(x)
-            x = tf.keras.layers.BatchNormalization()(x)
-            x = tf.keras.layers.Add()([tensor,x])
-            x = Swish(x)
-            
-            return x
-            
-        def projection_block(tensor , filters , strides):
-            x = conv_batch_relu(tensor , filters = filters , kernel_size = 1 , strides = strides)
-            x = conv_batch_relu(x , filters = filters , kernel_size = 3 , strides = 1)
-            x = tf.keras.layers.Conv2D(filters*4 , kernel_size = 1 , strides = 1)(x)
-            x = tf.keras.layers.BatchNormalization()(x)
-            
-            shortcut = tf.keras.layers.Conv2D(filters*4 , 1 , strides = strides)(tensor)
-            shortcut = tf.keras.layers.BatchNormalization()(shortcut)
-            
-            
-            x = tf.keras.layers.Add()([shortcut,x])
-            x = Swish(x)
-            return x
-        
-
-            
-
-        def res_main_block(x , filters ,reps , strides):
-            x = projection_block(x , filters , strides)
-            
-            for _ in range(reps-1):
-                x = identity_block(x , filters)
-            return x
-
-
-        inputs = tf.keras.layers.Input((img_H, img_W, channels))
-        
-        
-        x = tf.keras.layers.Conv2D(64, (7,7) , strides = (2,2) ,padding = "same")(inputs)
-        
-        x = tf.keras.layers.MaxPool2D((2,2))(x)
-        #x = tf.keras.layers.Conv2D(64*4, (1,1) , padding = "same")(x)
-        
-        x = res_main_block(x , 64 , 3 , strides = 1)
-        x = res_main_block(x , 128 , 4 , strides = 2)
-        x = res_main_block(x , 256 , 6 , strides = 2)
-        x = res_main_block(x , 512 , 3 , strides = 2)
-        
-        x = tf.keras.layers.GlobalAveragePooling2D()(x)
-
-        x = tf.keras.layers.Dense(256)(x)
-        x = tf.keras.layers.BatchNormalization()(x)
-        x = Swish(x)
-        
-        x = tf.keras.layers.Dense(128)(x)
-        x = tf.keras.layers.BatchNormalization()(x)
-        x = Swish(x)
-        
-        x = tf.keras.layers.Dense(64)(x)
-        x = tf.keras.layers.BatchNormalization()(x)
-        
-        x = tf.keras.layers.Dense(64)(x)
-        x = tf.keras.layers.BatchNormalization()(x)
-   
-    
-        outputs = tf.keras.layers.Dense(n_classes, activation='softmax')(x)
-        
-        model = tf.keras.Model(inputs=[inputs], outputs=[outputs])
-        return model 
-
-
-
-
-    @staticmethod
     def ResNet_50_Dropout(shape , n_classes):
         img_H , img_W , channels = shape
         
         def Swish(x):
             return x * tf.nn.sigmoid(x)  
 
         
@@ -1023,8 +611,56 @@
         x = tf.keras.layer.Activation('swish')(x)
         x = tf.keras.layers.Dropout(0.05*6)(x)
 
         
         outputs = tf.keras.layers.Dense(n_classes, activation='softmax')(x)
         model = tf.keras.Model(inputs=[inputs], outputs=[outputs])
         
-        return model
+        return model
+    
+    
+        
+    def SimpleMnist(shape = (28,28,1) , n_classes=10):
+        img_H , img_W , channels = shape
+    
+    
+        
+        inputs = tf.keras.layers.Input((img_H, img_W, channels))
+        def Conv_batch_swish(input_layer,channels,kernel,strides,dropout):
+            x = tf.keras.layers.Conv2D(channels,kernel,strides,padding = "same")(input_layer)
+            x = tf.keras.layers.BatchNormalization()(x)
+            x = tf.keras.layers.Activation('swish')(x)  
+            x = tf.keras.layers.Dropout(dropout)(x)
+            
+            return x
+            
+        def Dense_batch_swish(input_layer,channels,dropout):
+            x = tf.keras.layers.Dense(channels)(input_layer)
+            x = tf.keras.layers.BatchNormalization()(x)
+            x = tf.keras.layers.Activation('swish')(x)  
+            x = tf.keras.layers.Dropout(dropout)(x)
+            
+            return x
+            
+
+        x = Conv_batch_swish(inputs, channels = 32, kernel = 3, strides = 1, dropout = 0.1)
+        x = Conv_batch_swish(inputs, channels = 32, kernel = 3, strides = 2, dropout = 0.1)
+        
+        x = Conv_batch_swish(x, channels = 64, kernel = 3, strides = 1, dropout = 0.1)
+        x = Conv_batch_swish(x, channels = 64, kernel = 3, strides = 2, dropout = 0.1)
+        
+        x = Conv_batch_swish(x, channels = 128, kernel = 3, strides = 1, dropout = 0.1)
+
+
+        
+        x = tf.keras.layers.GlobalAveragePooling2D()(x)
+        
+        x = Dense_batch_swish(x, channels = 64, dropout = 0.3)
+        x = Dense_batch_swish(x, channels = 128, dropout = 0.5)
+        x = Dense_batch_swish(x, channels = 64, dropout = 0.3)
+    
+    
+    
+        outputs = tf.keras.layers.Dense(n_classes, activation='softmax')(x)
+    
+        model = tf.keras.Model(inputs=[inputs], outputs=[outputs])
+        return model
```

## NeuroUtils/Core.py

```diff
@@ -1,42 +1,54 @@
 #Downloading ml assets from library folder
-from NeuroUtils import ML_assets as ml
-from NeuroUtils import Architectures as arch
+import ML_assets as ml
+import Architectures as arch
 #Importing rest of the libraries
 import os
+import sys
 import tensorflow as tf
 import matplotlib.pyplot as plt
 import numpy as np
 from timeit import default_timer as timer   
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
 
 
 class Utils:
     
-    def Initialize_data(DataBase_directory, Data_directory, img_H, img_W, grayscale):
+    def Initialize_data(DataBase_directory, Data_directory, img_H, img_W, grayscale, Load_from_CSV):
     
         
         if not os.path.isdir(Data_directory):
             os.makedirs(Data_directory)
             print("Creating data storage directory...\n")
             
         if len(os.listdir(Data_directory)) == 0:
             print("There is no Dataset Initialized, initializing Dataset...")
-            ml.DataSets.Create_Img_Classification_DataSet(DataBase_directory, img_H, img_W, Save_directory=Data_directory , grayscale = grayscale)
+            if Load_from_CSV:
+                ml.DataSets.Create_Img_Classification_DataSet_CSV(DataBase_directory, img_H, img_W, Save_directory=Data_directory)
+            else:
+                ml.DataSets.Create_Img_Classification_DataSet(DataBase_directory, img_H, img_W, Save_directory=Data_directory , grayscale = grayscale)
         else:
             print("Found initialized Dataset")
             database_list = os.listdir(DataBase_directory)
             data_list = os.listdir(Data_directory)
+            if Load_from_CSV:
+                data_list = [element.replace(".csv" , "") for element in data_list] 
+                database_list = ['sample_submission', 'x_test','x_train', 'y_test','y_train']
+                
             data_list_clean = [element.replace(".npy" , "") for element in data_list] 
-    
+            
+            
             if database_list != data_list_clean:
                 print("Dataset is lacking some of the classes, initializing Dataset again")
-                ml.DataSets.Create_Img_Classification_DataSet(DataBase_directory, img_H, img_W, Save_directory=Data_directory , grayscale = grayscale)
+                if Load_from_CSV:
+                    ml.DataSets.Create_Img_Classification_DataSet_CSV(DataBase_directory, img_H, img_W, Save_directory=Data_directory)
+                else:
+                    ml.DataSets.Create_Img_Classification_DataSet(DataBase_directory, img_H, img_W, Save_directory=Data_directory , grayscale = grayscale)
             else:
                 print("Dataset is initialized correctly!")
                    
     
     def Process_Data(x , y ,dataset_multiplier, DataProcessed_directory, Kaggle_set, flipRotate = False , randBright = False , gaussian = False , denoise = False , contour = False ):        
         #Folder creation if not existing
         if not os.path.isdir(DataProcessed_directory):
@@ -71,28 +83,32 @@
         
                        
                 except:
                     print("Could not load processed files, probably not present in the folder, creating...")
                
     
         print("There is no Dataset processed, processing Dataset...")
-        print("Augmentation of images...")
-        if not (flipRotate and randBright and gaussian and denoise and contour) and dataset_multiplier >1:
-            print("\nNo augmentation specified, dataset will be just multiplied",dataset_multiplier, "times")
-            
-        if not (flipRotate and randBright and gaussian and denoise and contour) and dataset_multiplier <1:
-            print("\nNo augmentation, skipping...")
-        x,y = ml.DataSets.Augment_classification_dataset(x, y, dataset_multiplier, flipRotate, randBright, gaussian, denoise, contour )            
-        
+
         if Kaggle_set:
             x_train , x_val , y_train , y_val = train_test_split(x,y,test_size = 0.2 ,stratify = y, shuffle = True)
         else:
             x_train , x_val , y_train , y_val = train_test_split(x,y,test_size = 0.3 ,stratify = y, shuffle = True)
             x_val , x_test , y_val , y_test = train_test_split(x_val,y_val,test_size = 0.66 ,stratify = y_val, shuffle = True)
+        
+        print("Augmentation of images...")
+        if (not (flipRotate and randBright and gaussian and denoise and contour)) and dataset_multiplier >1:
+            print("\nNo augmentation specified, dataset will be just multiplied",dataset_multiplier, "times")
+            
+        if not (flipRotate and randBright and gaussian and denoise and contour) and dataset_multiplier <1:
+            print("\nNo augmentation, skipping...")
+        x_train,y_train = ml.DataSets.Augment_classification_dataset(x_train, y_train, dataset_multiplier, flipRotate, randBright, gaussian, denoise, contour )            
             
+        
+        
+        
         if not Kaggle_set:
             np.save(os.path.join(DataProcessed_directory ,"x_train.npy") , x_train)
             np.save(os.path.join(DataProcessed_directory ,"y_train.npy") , y_train)
             
             np.save(os.path.join(DataProcessed_directory ,"x_val.npy") , x_val)
             np.save(os.path.join(DataProcessed_directory ,"y_val.npy") , y_val)
             
@@ -134,24 +150,24 @@
         
         #!!! Building and compiling model
         #########################################################################
         #########################################################################
         #Choosing optimizer
         optimizer = tf.keras.optimizers.Adam()
         #Compiling model
-        model.compile(optimizer=optimizer, loss='categorical_crossentropy', metrics=['aUtilsuracy'])
+        model.compile(optimizer=optimizer, loss='categorical_crossentropy', metrics=['accuracy'])
         if show_architecture:
             model.summary()
         
         #########################################################################
         #########################################################################
         return model
     
         
-    def Initialize_weights_and_training(x_train, y_train, model, model_directory, model_architecture, train, epochs, patience, batch_size, x_val=None, y_val=None, device = "CPU:0"):    
+    def Initialize_weights_and_training(x_train, y_train, model, model_directory, model_architecture, train, epochs, patience, batch_size,min_delta, x_val=None, y_val=None, device = "CPU:0"):    
         #!!! Model training
         #########################################################################
         #########################################################################
         #Check if directory of trained model is present, if not, create one 
         if not os.path.isdir(model_directory):
             os.makedirs(model_directory)
             print("Creating model directory storage directory...\n")
@@ -172,15 +188,15 @@
             else:
                 csv_append = True
                 
             callbacks = [
                         #Stop if no increase in accuracy after x epochs
                         tf.keras.callbacks.EarlyStopping(patience=patience, 
                                                          monitor='val_accuracy',
-                                                         min_delta=0.01),
+                                                         min_delta=min_delta),
                         #Checkpoint model if performance is increased
                         tf.keras.callbacks.ModelCheckpoint(filepath = model_weights_directory  ,
                                                         monitor = "val_accuracy",
                                                         save_best_only = True,
                                                         verbose = 1),
                         #Save data through training
                         tf.keras.callbacks.CSVLogger(filename = model_history_directory , append = csv_append)
@@ -271,20 +287,23 @@
             except:
                 print("No test set provided, skipping...")
 
 class Project:
     class Classification_Project:
         def  __init__(self,config):
             #Low level constants
+            self.PROJECT_DIRECTORY = os.path.dirname(os.path.abspath(sys.argv[0]))
             #Initial
             self.DATABASE_DIRECTORY = config.Initial_params["DataBase_directory"]
             self.KAGGLE_SET = config.Initial_params["Kaggle_set"]
+            self.CSV_LOAD = config.Initial_params["Load_from_CSV"]
             self.IMG_H = config.Initial_params["img_H"]
             self.IMG_W = config.Initial_params["img_W"]
             self.GRAYSCALE= config.Initial_params["grayscale"]
+            self.DATA_TYPE = config.Initial_params["DataType"]
             
             #Augment
             self.REDUCED_SET_SIZE = config.Augment_params["reduced_set_size"]
             self.DATASET_MULTIPLIER = config.Augment_params["dataset_multiplier"]
             self.FLIPROTATE = config.Augment_params["flipRotate"]
             self.RANDBRIGHT = config.Augment_params["randBright"]
             self.GAUSSIAN = config.Augment_params["gaussian_noise"]
@@ -295,60 +314,79 @@
             self.MODEL_ARCHITECTURE = config.Model_parameters["model_architecture"]
             self.SHOW_ARCHITECTURE = config.Model_parameters["show_architecture"]
             self.DEVICE = config.Model_parameters["device"]
             self.TRAIN = config.Model_parameters["train"]
             self.EPOCHS = config.Model_parameters["epochs"]
             self.PATIENCE = config.Model_parameters["patience"]
             self.BATCH_SIZE = config.Model_parameters["batch_size"]
+            self.MIN_DELTA = config.Model_parameters["min_delta"]
             self.EVALUATE = config.Model_parameters["evaluate"]
             
             #High level constants
             #Form
             self.FORM = "Grayscale" if self.GRAYSCALE else "RGB"
             #Channels
             self.CHANNELS = 3 if self.FORM == "RGB" else 1
             self.CHANNELS = self.CHANNELS+1 if self.CONTOUR else self.CHANNELS
     
             self.PARAM_MARK = "__" + "_".join(["1" if x else "0" for x in [self.FLIPROTATE, self.RANDBRIGHT, self.GAUSSIAN, self.DENOISE, self.CONTOUR]])
     
                     
-            self.DATA_DIRECTORY = os.path.join(os.path.dirname(os.path.realpath(__file__)) , "DataSet" , str(str(self.IMG_H)+"x"+str(self.IMG_W)+"_"+self.FORM))
-            self.DATAPROCESSED_DIRECTORY = os.path.join(os.path.dirname(os.path.realpath(__file__)) , "DataSet_Processed" , str(str(self.IMG_H)+"x"+str(self.IMG_W)+"_"+self.FORM),self.PARAM_MARK)
-            self.MODEL_DIRECTORY =  os.path.join(os.path.dirname(os.path.realpath(__file__)) , "Models_saved" , str(self.MODEL_ARCHITECTURE) , self.FORM , str(str(self.IMG_H)+"x"+str(self.IMG_W)) , str("bs"+str(self.BATCH_SIZE) + self.PARAM_MARK)  )
-    
+            self.DATA_DIRECTORY = os.path.join(self.PROJECT_DIRECTORY , "DataSet" , str(str(self.IMG_H)+"x"+str(self.IMG_W)+"_"+self.FORM))
+            self.DATAPROCESSED_DIRECTORY = os.path.join(self.PROJECT_DIRECTORY , "DataSet_Processed" , str(str(self.IMG_H)+"x"+str(self.IMG_W)+"_"+self.FORM),self.PARAM_MARK)
+            self.MODEL_DIRECTORY =  os.path.join(self.PROJECT_DIRECTORY , "Models_saved" , str(self.MODEL_ARCHITECTURE) , self.FORM , str(str(self.IMG_H)+"x"+str(self.IMG_W)) , str("bs"+str(self.BATCH_SIZE) + self.PARAM_MARK)  )
             
             
             
             
         def __str__(self):
             return f"This is class representing the project, main parameters are:\n\nOriginalDatabase: {self.DATABASE_DIRECTORY}\nArchitecture Used: {self.MODEL_ARCHITECTURE}"
             
     
         def Initialize_data(self): 
             """Initializing dataset from main database folder with photos to project folder in numpy format. Photos are 
             Resized and cropped without loosing much aspect ratio, r parameter decides above what proportions of edges 
             image will be cropped to square instead of squeezed""" 
             
-            Utils.Initialize_data(self.DATABASE_DIRECTORY, self.DATA_DIRECTORY, self.IMG_H, self.IMG_W, self.GRAYSCALE)
+            Utils.Initialize_data(self.DATABASE_DIRECTORY, self.DATA_DIRECTORY, self.IMG_H, self.IMG_W, self.GRAYSCALE , self.CSV_LOAD)
             ########################################################
         def Load_and_merge_data(self):
             """Loading dataset to memory from data directory in project folder, sets can be reduced to equal size
             to eliminate disproportions if they are not same size at the main database
             In this module dictionary with names of classes is created as well, names are based on names of datsets
             Datasets names are based on the folder names in main database folder"""
             
             self.X_TRAIN, self.Y_TRAIN, self.DICTIONARY = ml.DataSets.Load_And_Merge_DataSet(self.DATA_DIRECTORY , self.REDUCED_SET_SIZE )
             self.N_CLASSES = len(self.DICTIONARY)
             ########################################################
             
         def Process_data(self):
             #3
             ########################################################
-            self.X_TRAIN , self.Y_TRAIN, self.X_VAL , self.Y_VAL , self.X_TEST , self.Y_TEST = Utils.Process_Data(self.X_TRAIN, self.Y_TRAIN, self.DATASET_MULTIPLIER, self.DATAPROCESSED_DIRECTORY, self.KAGGLE_SET, self.FLIPROTATE, self.RANDBRIGHT, self.GAUSSIAN, self.DENOISE, self.CONTOUR)
+            if self.KAGGLE_SET:
+                self.X_TRAIN , self.Y_TRAIN, self.X_VAL , self.Y_VAL = Utils.Process_Data(self.X_TRAIN, self.Y_TRAIN, self.DATASET_MULTIPLIER, self.DATAPROCESSED_DIRECTORY, self.KAGGLE_SET, self.FLIPROTATE, self.RANDBRIGHT, self.GAUSSIAN, self.DENOISE, self.CONTOUR)
+            
+            else:
+                self.X_TRAIN , self.Y_TRAIN, self.X_VAL , self.Y_VAL , self.X_TEST , self.Y_TEST = Utils.Process_Data(self.X_TRAIN, self.Y_TRAIN, self.DATASET_MULTIPLIER, self.DATAPROCESSED_DIRECTORY, self.KAGGLE_SET, self.FLIPROTATE, self.RANDBRIGHT, self.GAUSSIAN, self.DENOISE, self.CONTOUR)
+            
+            try:
+                self.X_TRAIN = np.array(self.X_TRAIN/255 , dtype = self.DATA_TYPE)
+                self.Y_TRAIN = np.array(self.Y_TRAIN , dtype = self.DATA_TYPE)
+                
+                self.X_VAL = np.array(self.X_VAL/255 , dtype = self.DATA_TYPE)
+                self.Y_VAL = np.array(self.Y_VAL , dtype = self.DATA_TYPE)
+                
+                self.X_TEST = np.array(self.X_TEST/255 , dtype = self.DATA_TYPE)
+                self.Y_TEST = np.array(self.Y_TEST , dtype = self.DATA_TYPE)
+            except Exception as e:
+                print("Could not standarize data:",e)
+            
+            
             ########################################################
+            
     
         def Initialize_model_from_library(self):
             #4
             ########################################################
             self.MODEL = Utils.Initialize_model(model_architecture = self.MODEL_ARCHITECTURE,
                                         n_classes = self.N_CLASSES,
                                         img_H = self.IMG_H,
@@ -378,14 +416,15 @@
                                                        model = self.MODEL,
                                                        model_directory = self.MODEL_DIRECTORY,
                                                        model_architecture = self.MODEL_ARCHITECTURE,
                                                        train = self.TRAIN,
                                                        epochs = self.EPOCHS,
                                                        patience = self.PATIENCE,
                                                        batch_size = self.BATCH_SIZE,
+                                                       min_delta= self.MIN_DELTA,
                                                        device = self.DEVICE
                                                        )
             ########################################################
     
         def Initialize_resulits(self):
             #6
             ########################################################
@@ -397,8 +436,19 @@
                                   self.Y_TRAIN,
                                   self.X_VAL,
                                   self.Y_VAL,
                                   self.X_TEST,
                                   self.Y_TEST
                                   )
             ######################################################## 
+            
+        def Generate_sample_submission(self, filepath = None):
+            if filepath is None:
+                sample_submission = pd.read_csv(os.path.join(self.DATA_DIRECTORY , "sample_submission.csv")) 
+
+            #img_id = sample_submission.columns[0]
+            label = sample_submission.columns[1]
+
+            label_array = np.argmax(self.MODEL.predict(self.X_TEST), axis = 1)
+            sample_submission[label] = label_array
+            return sample_submission
```

## NeuroUtils/ML_assets.py

```diff
@@ -147,15 +147,72 @@
         
         
 
               
         
         
         print("----------------------\nTime took compiling images:",round(timer()-timer_start,2),"\n----------------------")
-        
+
+
+    def Create_Img_Classification_DataSet_CSV(Database_directory , img_H , img_W, Save_directory):
+        Set_list  = os.listdir(Database_directory)
+
+        for Set in Set_list:
+            try:
+                directory = os.path.join(Database_directory , str(Set))
+                data = pd.read_csv(directory)
+                #Save dataframe directly into data folder if its sample submission
+                if str(Set) == "sample_submission.csv":
+                    data.to_csv(os.path.join(Save_directory , Set),index =False)
+                    continue
+                    
+                #Checking if label is present in data, it indicates its not test data
+                if 'label' in data.columns:
+                    labels = np.array(data["label"].values , dtype = int)
+                    y = General.OneHot_decode(labels)
+                    data.drop(columns=['label'], inplace=True)
+                
+                else:
+                    y = None    
+                lenght = len(data.iloc[0,:].values)
+                
+                if img_H*img_W == lenght:
+                    
+                    x = []
+                    description = str("Preparing "+Set)
+                    for k in tqdm(range(len(data)) , desc = description):
+                        img = np.zeros((img_H,img_W),dtype = np.uint8)
+                        for i in range(img_H):
+                            img[i,:] = data.iloc[k,i*img_W:(i+1)*img_W]
+                        x.append(img)
+                    x = np.array(x)
+                    
+                    
+                    
+                    
+                    x_set_save_dir = str("x_"+str(Set.replace(".csv",""))+".npy")
+                    y_set_save_dir = str("y_"+str(Set.replace(".csv",""))+".npy")
+                    
+                    np.save(os.path.join(Save_directory , x_set_save_dir), x)
+                    np.save(os.path.join(Save_directory , y_set_save_dir), y)
+                    
+                    #Making list of sets which are done #2
+                    print("Done")
+                    print("----------------------------------------------")
+                    
+                    
+                    
+                else:
+                    print("Mismatch in provided image resolution and expected one. By default if square it should be:",img_H,"x",img_W)
+            
+            except Exception as e:
+                #Print Exception
+                print("\nCould not load file: ", Set)
+                print(e)
+          
        
         
             
     def Load_And_Merge_DataSet(Data_directory , samples_per_class = None):
 
         Classes_list  = os.listdir(Data_directory)
         n_classes = len(Classes_list)
@@ -195,19 +252,21 @@
         return x , ClassSet , Dictionary
             
             
               
 
     def Augment_classification_dataset(x, y, dataset_multiplier, flipRotate = False , randBright = False , gaussian = False , denoise = False , contour = False ):
         n_classes = y.shape[1]
-    
         lenght = x.shape[0]
         img_H = x.shape[1]
         img_W = x.shape[2]
-        channels = x.shape[3]
+        try:
+            channels = x.shape[3]
+        except:
+            channels = 1
         
         blank_class_y = np.zeros((0,n_classes) , dtype = np.uint8)
         if channels == 1:
             blank_class_x = np.zeros((0,img_H,img_W) , dtype = np.uint8)
         else:
             blank_class_x = np.zeros((0,img_H,img_W,channels) , dtype = np.uint8)
             
@@ -410,15 +469,15 @@
                 starting_epoch = Model_history["epoch"].iloc[-1]
                 best_val_acc = Model_history["val_accuracy"].idxmax()
                 
                 best_val_loss = round(Model_history["val_loss"][best_val_acc],3)
                 best_val_acc = round(Model_history["val_accuracy"][best_val_acc],3)
         
                 print("Found existing model trained for ",starting_epoch," epochs")
-                print("Best model score aqcuired in ",starting_epoch," epoch\nVal_acc: ",best_val_acc,"\nVal_loss: ",best_val_acc,)
+                print("Best model score aqcuired in ",starting_epoch," epoch\nVal_acc: ",best_val_acc,"\nVal_loss: ",best_val_loss,)
                 
                 print("Do you want to continue training? \nType 'y' for yes and 'n' for no \n")
                 user_input = input()
         
                 while True:
                     if user_input.lower() =="y":
                         print("Continuing model training")
```

## Comparing `NeuroUtils-0.1.3.dist-info/LICENSE.txt` & `NeuroUtils-0.1.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `NeuroUtils-0.1.3.dist-info/METADATA` & `NeuroUtils-0.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroUtils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library for neural network projects organisation
 Author-email: Sebastian Borukało <Ciapserr@gmail.com>
 Project-URL: Homepage, https://github.com/Ciapser/NeuroUtils
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
```

## Comparing `NeuroUtils-0.1.3.dist-info/RECORD` & `NeuroUtils-0.1.4.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-NeuroUtils/Architectures.py,sha256=Xy6JTKyR41gMMdR8P1ByeuIPT6hGgA4cQONbptVXCVk,38839
-NeuroUtils/Core.py,sha256=sVdb6Rg9Fk1CUjTx22qd6jS6fShICCcHeLxtjCafa1I,21193
-NeuroUtils/ML_assets.py,sha256=o7etZb7uRJfNdyQ_kkG5HsUo2Gg6fwZJAx7KYBliEo8,22147
+NeuroUtils/Architectures.py,sha256=aWofjCgpJ5epv0vpF6joYOOn_fFggvsukZ_Pqoxzl4c,25630
+NeuroUtils/Core.py,sha256=FLlErOne7-lyGeBkXpBOWccdRvjb2JYlirNjOzQSMxA,23725
+NeuroUtils/ML_assets.py,sha256=8m5RX-leIl-Ni0ihmhjb8tbuL4cpbMForamO7qkYSew,24791
 NeuroUtils/__init__.py,sha256=M19PlxWTqxnYsQc03A3XCzFoFFNRpV0uBG0B-76TLBQ,50
-NeuroUtils-0.1.3.dist-info/LICENSE.txt,sha256=aUncEakBCK32RA3QKKi4TV-y1cb4gwGer68lX2Z7NBE,571
-NeuroUtils-0.1.3.dist-info/METADATA,sha256=opCK1srLm9QnsNdJxk63bnfC89GLC02AgjMbb-rqDFA,2078
-NeuroUtils-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-NeuroUtils-0.1.3.dist-info/top_level.txt,sha256=1PAx5XIE5jUM7BcxFhiGFXZ0ZpFhT5BzUQn8nwtSs_Q,11
-NeuroUtils-0.1.3.dist-info/RECORD,,
+NeuroUtils-0.1.4.dist-info/LICENSE.txt,sha256=aUncEakBCK32RA3QKKi4TV-y1cb4gwGer68lX2Z7NBE,571
+NeuroUtils-0.1.4.dist-info/METADATA,sha256=4MWn2fO_OraAHBeRWKf9IHePd_ciOLCD-m-UHABPWvg,2078
+NeuroUtils-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+NeuroUtils-0.1.4.dist-info/top_level.txt,sha256=1PAx5XIE5jUM7BcxFhiGFXZ0ZpFhT5BzUQn8nwtSs_Q,11
+NeuroUtils-0.1.4.dist-info/RECORD,,
```

