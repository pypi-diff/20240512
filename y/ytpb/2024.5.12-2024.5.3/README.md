# Comparing `tmp/ytpb-2024.5.12.tar.gz` & `tmp/ytpb-2024.5.3.tar.gz`

## Comparing `ytpb-2024.5.12.tar` & `ytpb-2024.5.3.tar`

### file list

```diff
@@ -1,182 +1,140 @@
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ytpb-2024.5.12/.gitattributes
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ytpb-2024.5.12/.pre-commit-config.yaml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ytpb-2024.5.12/.readthedocs.yaml
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 ytpb-2024.5.12/CHANGELOG.md
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ytpb-2024.5.12/CONTRIBUTING.rst
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ytpb-2024.5.12/Makefile
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 ytpb-2024.5.12/config.toml.example
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/changelog.rst
--rw-r--r--   0        0        0    24143 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/cli.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/contributing.rst
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/cookbook.rst
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/index.rst
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/quick.rst
--rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/reference.rst
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/why.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/_templates/sidebarintro.html
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/index.rst
--rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/usage.rst
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/index.rst
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.actions.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.cache.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.download.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.errors.rst
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.fetchers.rst
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.info.rst
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.locate.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.merge.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.playback.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.representations.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.segment.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.5.12/docs/package/api/ytpb.streams.rst
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 ytpb-2024.5.12/etc/0001-Revert-http-Send-a-Range-header-even-when-the-offset.patch
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 ytpb-2024.5.12/etc/0002-Revert-http-Improve-handling-of-Content-Range-with-T.patch
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 ytpb-2024.5.12/etc/Containerfile
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/__main__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/_version.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/api.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/cache.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/conditional.py
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/config.py
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/download.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/errors.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/fetchers.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/info.py
--rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/locate.py
--rw-r--r--   0        0        0    13308 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/merge.py
--rw-r--r--   0        0        0    23900 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/playback.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/representations.py
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/segment.py
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/streams.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/types.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/actions/__init__.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/actions/capture.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/actions/compose.py
--rw-r--r--   0        0        0     7755 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/actions/download.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/cli/__init__.py
--rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/cli/common.py
--rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/cli/options.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/cli/parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/cli/commands/__init__.py
--rw-r--r--   0        0        0    17114 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/cli/commands/capture.py
--rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/cli/commands/download.py
--rw-r--r--   0        0        0    10381 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/cli/commands/mpd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/utils/__init__.py
--rw-r--r--   0        0        0     8090 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/utils/date.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/utils/ffmpeg.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/utils/other.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/utils/path.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/utils/remote.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 ytpb-2024.5.12/src/ytpb/utils/url.py
--rw-r--r--   0        0        0     9242 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/conftest.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/helpers.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_cache.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_download.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_fetchers.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_info.py
--rw-r--r--   0        0        0     7991 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_locate.py
--rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_merge.py
--rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_playback.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_playback_session.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_representations.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_segment.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_streams.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/actions/__init__.py
--rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/actions/test_compose.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/actions/test_download.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/cli/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/cli/conftest.py
--rw-r--r--   0        0        0    60744 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/cli/test_download_command.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/cli/test_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/cli/capture/__init__.py
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/cli/capture/test_frame_command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/cli/mpd/__init__.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/cli/mpd/test_compose_command.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/cli/mpd/test_refresh_command.py
--rw-r--r--   0        0        0    56372 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/info-1695928670.json
--rw-r--r--   0        0        0  2978627 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/manifest-1695928670.mpd
--rw-r--r--   0        0        0   701494 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/webpage-1695928670.html
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244]-Darwin.out
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244]-Linux.out
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244]-Windows.out
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-none]-Darwin.out
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-none]-Linux.out
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-none]-Windows.out
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244]-Darwin.out
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244]-Linux.out
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244]-Windows.out
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd_with_no_streams-Darwin.out
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd_with_no_streams-Linux.out
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_compose_mpd_with_no_streams-Windows.out
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244]-Darwin.out
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244]-Linux.out
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244]-Windows.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none]-Darwin.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none]-Linux.out
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none]-Windows.out
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244]-Darwin.out
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244]-Linux.out
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244]-Windows.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4]-Darwin.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4]-Linux.out
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4]-Windows.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4]-Darwin.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4]-Linux.out
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4]-Windows.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4]-Darwin.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4]-Linux.out
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4]-Windows.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4]-Darwin.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4]-Linux.out
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4]-Windows.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4]-Darwin.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4]-Linux.out
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4]-Windows.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4]-Darwin.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4]-Linux.out
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4]-Windows.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4]-Darwin.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4]-Linux.out
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4]-Windows.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4]-Darwin.out
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4]-Linux.out
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4]-Windows.out
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_dry_run_option-Darwin.out
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_dry_run_option-Linux.out
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_dry_run_option-Windows.out
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_no_cut_option-Darwin.out
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_no_cut_option-Linux.out
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_no_cut_option-Windows.out
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_no_merge_option-Darwin.out
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_no_merge_option-Linux.out
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_no_merge_option-Windows.out
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_refresh_mpd-Darwin.out
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_refresh_mpd-Linux.out
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/expected/test_refresh_mpd-Windows.out
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/gap-cases/gap-case-1-fixture.csv
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/gap-cases/gap-case-2-fixture.csv
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/gap-cases/gap-case-3-fixture.csv
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/segments/7959120.i140.mp4
--rw-r--r--   0        0        0   172355 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/segments/7959120.i244.webm
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/segments/7959121.i140.mp4
--rw-r--r--   0        0        0   171647 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/segments/7959121.i244.webm
--rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/segments/7959122.i140.mp4
--rw-r--r--   0        0        0   173730 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/segments/7959122.i244.webm
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/segments/7959123.i140.mp4
--rw-r--r--   0        0        0   172126 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/segments/7959123.i244.webm
--rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/segments/7959203.i140.mp4
--rw-r--r--   0        0        0   172036 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/data/segments/7959203.i244.webm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/utils/__init__.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/utils/test_date.py
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/utils/test_path.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/utils/test_remote.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ytpb-2024.5.12/tests/utils/test_url.py
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 ytpb-2024.5.12/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb-2024.5.12/LICENSE
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 ytpb-2024.5.12/README.rst
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 ytpb-2024.5.12/pyproject.toml
--rw-r--r--   0        0        0     7364 2020-02-02 00:00:00.000000 ytpb-2024.5.12/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.gitattributes
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 ytpb-2024.5.3/CHANGELOG.rst
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ytpb-2024.5.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ytpb-2024.5.3/Makefile
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 ytpb-2024.5.3/config.toml.example
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/changelog.rst
+-rw-r--r--   0        0        0    24143 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/cli.rst
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/contributing.rst
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/cookbook.rst
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/index.rst
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/quick.rst
+-rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/reference.rst
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/why.rst
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/index.rst
+-rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/usage.rst
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/index.rst
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.actions.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.cache.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.download.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.errors.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.fetchers.rst
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.info.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.locate.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.merge.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.playback.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.representations.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.segment.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.5.3/docs/package/api/ytpb.streams.rst
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 ytpb-2024.5.3/etc/Containerfile
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/__main__.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/api.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cache.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/conditional.py
+-rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/config.py
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/download.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/errors.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/fetchers.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/ffmpeg.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/info.py
+-rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/locate.py
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/merge.py
+-rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/playback.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/representations.py
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/segment.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/streams.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/types.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/__init__.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/capture.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/compose.py
+-rw-r--r--   0        0        0     7755 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/actions/download.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/__init__.py
+-rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/common.py
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/options.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/__init__.py
+-rw-r--r--   0        0        0    17114 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/capture.py
+-rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/download.py
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/cli/commands/mpd.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/__init__.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/date.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/other.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/path.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/remote.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 ytpb-2024.5.3/src/ytpb/utils/url.py
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/conftest.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/helpers.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_cache.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_download.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_fetchers.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_info.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_locate.py
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_merge.py
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_playback.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_playback_session.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_representations.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_segment.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_streams.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/actions/__init__.py
+-rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/actions/test_compose.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/actions/test_download.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/conftest.py
+-rw-r--r--   0        0        0    60600 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/test_download_command.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/test_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/capture/__init__.py
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/capture/test_frame_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/mpd/__init__.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/mpd/test_compose_command.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/cli/mpd/test_refresh_command.py
+-rw-r--r--   0        0        0    56372 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/info-1695928670.json
+-rw-r--r--   0        0        0  2978627 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/manifest-1695928670.mpd
+-rw-r--r--   0        0        0   701494 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/webpage-1695928670.html
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_compose_mpd_with_no_streams.out
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_dry_run_option.out
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_no_cut_option.out
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_no_merge_option.out
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/expected/test_refresh_mpd.out
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/gap-cases/gap-case-1-fixture.csv
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/gap-cases/gap-case-2-fixture.csv
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/gap-cases/gap-case-3-fixture.csv
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959120.i140.mp4
+-rw-r--r--   0        0        0   172355 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959120.i244.webm
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959121.i140.mp4
+-rw-r--r--   0        0        0   171647 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959121.i244.webm
+-rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959122.i140.mp4
+-rw-r--r--   0        0        0   173730 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959122.i244.webm
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959123.i140.mp4
+-rw-r--r--   0        0        0   172126 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959123.i244.webm
+-rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959203.i140.mp4
+-rw-r--r--   0        0        0   172036 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/data/segments/7959203.i244.webm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/__init__.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_date.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_path.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_remote.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ytpb-2024.5.3/tests/utils/test_url.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 ytpb-2024.5.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb-2024.5.3/LICENSE
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 ytpb-2024.5.3/README.rst
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 ytpb-2024.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 ytpb-2024.5.3/PKG-INFO
```

### Comparing `ytpb-2024.5.12/CHANGELOG.md` & `ytpb-2024.5.3/CHANGELOG.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,106 +1,105 @@
-# Changelog
+Changelog
+#########
 
-Versions follow [Calendar Versioning](https://calver.org) with the `YYYY.M.D`
-scheme.
+Versions follow `Calendar Versioning`_ with the ``YYYY.M.D`` scheme.
 
-## [2024.5.12]
+.. _Calendar Versioning: https://calver.org
 
-- Add Windows support ([#11](https://github.com/xymaxim/ytpb/issues/11))
-- Fix not cutting issue introduced in v2024.5.3
-  ([b0e4f3d](https://github.com/xymaxim/ytpb/commit/b0e4f3d10c6aad7401716f49e681bb97c2ee6d03))
-- Replace all `ffprobe` calls to `av`'s function calls
-- Move `ytpb.ffmpeg` to `ytpb.utils.ffmpeg`
-- Add CI workflows to create test expectation files, build Windows binaries,
-  publish on PyPI, and draft a GitHub release
-- Run CI tests on Linux, MacOS, and Windows
-- Start using dynamic versioning via `hatch-vcs`
-- Convert CHANGELOG from ReST to Markdown format
-- Apply patches from files in Containerfile to avoid merge conflicts
+`2024.5.3`_
+***********
 
-## [2024.5.3]
-
-- Add support for resumable downloads
-  ([#13](https://github.com/xymaxim/ytpb/pull/13))
+- Add support for resumable downloads (`#13
+  <https://github.com/xymaxim/ytpb/pull/13>`__)
 - Change the segments output directory from the run temporary directory to a
   directory under the current working one
-- Add `--ignore-resume`, `-S / --keep-segments`, and `--segments-output-dir`
-  options
-- Change the default output path to `<title>_<id>_<input_start_date>`
-- Rename the `--no-cleanup` option to `--keep-temp`
-- Replace the `--preview` option with `--preview-start` and `--preview-end`
+- Add ``--ignore-resume``, ``-S / --keep-segments``, and
+  ``--segments-output-dir`` options
+- Change the default output path to ``<title>_<id>_<input_start_date>``
+- Rename the ``--no-cleanup`` option to ``--keep-temp``
+- Replace the ``--preview`` option with ``--preview-start`` and
+  ``--preview-end``
 
-## [2024.4.20]
+`2024.4.20`_
+************
 
 - Fix wrong frame rate values of the video-only merged files when boundary
-  segments are cut and encoded with H.264
-  ([e1120bf](https://github.com/xymaxim/ytpb/commit/e1120bf4514333ff3ac5d4eac862ccb6a9d5f606))
-- Write metadata tags with basic and rewind information to merged files
-  ([aa7adf1](https://github.com/xymaxim/ytpb/commit/aa7adf1580e5a83c9abaa76f2836b9a0570cc4ba))
-- Add the `--no-metadata` option to not write metadata tags to merged files
-
-## [2024.4.12]
-
-- Add the [Python
-  package](https://ytpb.readthedocs.io/en/latest/package/index.html) page with
-  the basic usage and API reference
-- Add the `--version` CLI option to show version number
-- Add `ytpb.representations.RepresentationInfo.type` property
-- Add `ytpb.playback.RewindInterval.duration` and
-  `ytpb.playback.RewindInterval.sequences` properties
-- Accept Unix timestamps for moments and intervals
-  ([b7dcbaf](https://github.com/xymaxim/ytpb/commit/b7dcbaf6eebe3f6022b7fa8eefe98f4b8af7c4cb))
-- Add `ytpb.playback.RewindTreeMap` to keep rewind history
-  ([91fd078](https://github.com/xymaxim/ytpb/commit/91fd078caf37f31fee167e0c2a20a38aa2badcd8))
-
-### Breaking changes
-
-- Rename `ytpb.mpd` to `ytpb.representations`
-- Rename `ytpb.exceptions` to `ytpb.errors`
-- Rename `ytpb.playback.Playback.get_downloaded_segment` to
-  `ytpb.playback.Playback.get_segment`
-- Rename `ytpb.representations.extract_representations_info` to
-  `ytpb.representations.extract_representations`
-- Remove unused `ytpb.representations.strip_manifest`
+  segments are cut and encoded with H.264 (`e1120bf
+  <https://github.com/xymaxim/ytpb/commit/e1120bf4514333ff3ac5d4eac862ccb6a9d5f606>`__)
+- Write metadata tags with basic and rewind information to merged files (`aa7adf1
+  <https://github.com/xymaxim/ytpb/commit/aa7adf1580e5a83c9abaa76f2836b9a0570cc4ba>`__)
+- Add the ``--no-metadata`` option to not write metadata tags to merged files
+
+`2024.4.12`_
+************
+
+- Add the `Python package
+  <https://ytpb.readthedocs.io/en/latest/package/index.html>`__ page with the
+  basic usage and API reference
+- Add the ``--version`` CLI option to show version number
+- Add :attr:`ytpb.representations.RepresentationInfo.type` property
+- Add :attr:`ytpb.playback.RewindInterval.duration` and
+  :attr:`~ytpb.playback.RewindInterval.sequences` properties
+- Accept Unix timestamps for moments and intervals (`b7dcbaf
+  <https://github.com/xymaxim/ytpb/commit/b7dcbaf6eebe3f6022b7fa8eefe98f4b8af7c4cb>`__)
+- Add :class:`ytpb.playback.RewindTreeMap` to keep rewind history (`91fd078
+  <https://github.com/xymaxim/ytpb/commit/91fd078caf37f31fee167e0c2a20a38aa2badcd8>`__)
+
+Breaking changes
+================
+
+- Rename :mod:`ytpb.mpd` to :mod:`ytpb.representations`
+- Rename :mod:`ytpb.exceptions` to :mod:`ytpb.errors`
+- Rename :meth:`ytpb.playback.Playback.get_downloaded_segment` to
+  :meth:`~ytpb.playback.Playback.get_segment`
+- Rename :meth:`ytpb.representations.extract_representations_info` to
+  :meth:`~ytpb.representations.extract_representations`
+- Remove unused :meth:`ytpb.representations.strip_manifest`
 
-## [2024.3.27]
+`2024.3.27`_
+************
 
 - Add Containerfile with instructions to build patched FFmpeg and MPV
 
-### Breaking changes
+Breaking changes
+================
+
+- Change return value of
+  :meth:`ytpb.locate.SegmentLocator.find_sequence_by_time` to
+  :class:`~ytpb.locate.LocateResult`
 
-- Change return value of `ytpb.locate.SegmentLocator.find_sequence_by_time` to
-  `ytpb.locate.LocateResult`
+`2024.3.16`_
+************
 
-## [2024.3.16]
+- Add options to dump base (``--dump-base-urls``) and segment
+  (``--dump-segment-urls``) URLs to the ``download`` command (`#10
+  <https://github.com/xymaxim/ytpb/pull/10>`__)
+- Add the `Cookbook`_ documentation page
 
-- Add options to dump base (`--dump-base-urls`) and segment
-  (`--dump-segment-urls`) URLs to the `download` command
-  ([#10](https://github.com/xymaxim/ytpb/pull/10))
-- Add the [Cookbook](https://ytpb.readthedocs.io/en/latest/cookbook.html)
-  documentation page
+.. _Cookbook: https://ytpb.readthedocs.io/en/latest/cookbook.html
 
-## [2024.3.13]
+`2024.3.13`_
+************
 
 - Add the config.toml.example file
-- Add ability to use [custom
-  aliases](https://ytpb.readthedocs.io/en/latest/reference.html#custom-aliases)
-  in format specs
-- Add [aliases](https://ytpb.readthedocs.io/en/latest/reference.html#itags) for
-  itags (`@<itag>`) as [dynamic
-  aliases](https://ytpb.readthedocs.io/en/latest/reference.html#aliases)
+- Add ability to use `custom aliases`_ in format specs
+- Add `aliases`_ for itags (``@<itag>``) as `dynamic aliases`_
 - Fix allowing empty representations in the CLI commands
 
-## [2024.3.9]
+.. _custom aliases: https://ytpb.readthedocs.io/en/latest/reference.html#custom-aliases
+.. _aliases: https://ytpb.readthedocs.io/en/latest/reference.html#itags
+.. _dynamic aliases: https://ytpb.readthedocs.io/en/latest/reference.html#aliases
+
+`2024.3.9`_
+***********
 
 - Add the CHANGELOG file and documentation page
-- Change the first segment locating step: don\'t limit it to two jumps
-  ([#8](https://github.com/xymaxim/ytpb/pull/8))
+- Change the first segment locating step: don't limit it to two jumps (`#8
+  <https://github.com/xymaxim/ytpb/pull/8>`__)
 
-[2024.5.12]: https://github.com/xymaxim/ytpb/compare/v2024.5.3..v2024.5.12
-[2024.5.3]: https://github.com/xymaxim/ytpb/compare/v2024.4.20..v2024.5.3
-[2024.4.20]: https://github.com/xymaxim/ytpb/compare/v2024.4.12..v2024.4.20
-[2024.4.12]: https://github.com/xymaxim/ytpb/compare/v2024.3.27..v2024.4.12
-[2024.3.27]: https://github.com/xymaxim/ytpb/compare/v2024.3.16..v2024.3.27
-[2024.3.16]: https://github.com/xymaxim/ytpb/compare/v2024.3.13..v2024.3.16
-[2024.3.13]: https://github.com/xymaxim/ytpb/compare/v2024.3.9..v2024.3.13
-[2024.3.9]: https://github.com/xymaxim/ytpb/compare/v2024.3.7..v2024.3.9
+.. _2024.5.3: https://github.com/xymaxim/ytpb/compare/v2024.4.20..v2024.5.3
+.. _2024.4.20: https://github.com/xymaxim/ytpb/compare/v2024.4.12..v2024.4.20
+.. _2024.4.12: https://github.com/xymaxim/ytpb/compare/v2024.3.27..v2024.4.12
+.. _2024.3.27: https://github.com/xymaxim/ytpb/compare/v2024.3.16..v2024.3.27
+.. _2024.3.16: https://github.com/xymaxim/ytpb/compare/v2024.3.13..v2024.3.16
+.. _2024.3.13: https://github.com/xymaxim/ytpb/compare/v2024.3.9..v2024.3.13
+.. _2024.3.9: https://github.com/xymaxim/ytpb/compare/v2024.3.7..v2024.3.9
```

#### html2text {}

```diff
@@ -1,61 +1,56 @@
-# Changelog Versions follow [Calendar Versioning](https://calver.org) with the
-`YYYY.M.D` scheme. ## [2024.5.12] - Add Windows support ([#11](https://
-github.com/xymaxim/ytpb/issues/11)) - Fix not cutting issue introduced in
-v2024.5.3 ([b0e4f3d](https://github.com/xymaxim/ytpb/commit/
-b0e4f3d10c6aad7401716f49e681bb97c2ee6d03)) - Replace all `ffprobe` calls to
-`av`'s function calls - Move `ytpb.ffmpeg` to `ytpb.utils.ffmpeg` - Add CI
-workflows to create test expectation files, build Windows binaries, publish on
-PyPI, and draft a GitHub release - Run CI tests on Linux, MacOS, and Windows -
-Start using dynamic versioning via `hatch-vcs` - Convert CHANGELOG from ReST to
-Markdown format - Apply patches from files in Containerfile to avoid merge
-conflicts ## [2024.5.3] - Add support for resumable downloads ([#13](https://
-github.com/xymaxim/ytpb/pull/13)) - Change the segments output directory from
-the run temporary directory to a directory under the current working one - Add
-`--ignore-resume`, `-S / --keep-segments`, and `--segments-output-dir` options
-- Change the default output path to `
-_` - Rename the `--no-cleanup` option to `--keep-temp` - Replace the `--
-preview` option with `--preview-start` and `--preview-end` ## [2024.4.20] - Fix
-wrong frame rate values of the video-only merged files when boundary segments
-are cut and encoded with H.264 ([e1120bf](https://github.com/xymaxim/ytpb/
-commit/e1120bf4514333ff3ac5d4eac862ccb6a9d5f606)) - Write metadata tags with
-basic and rewind information to merged files ([aa7adf1](https://github.com/
-xymaxim/ytpb/commit/aa7adf1580e5a83c9abaa76f2836b9a0570cc4ba)) - Add the `--no-
-metadata` option to not write metadata tags to merged files ## [2024.4.12] -
-Add the [Python package](https://ytpb.readthedocs.io/en/latest/package/
-index.html) page with the basic usage and API reference - Add the `--version`
-CLI option to show version number - Add
-`ytpb.representations.RepresentationInfo.type` property - Add
-`ytpb.playback.RewindInterval.duration` and
-`ytpb.playback.RewindInterval.sequences` properties - Accept Unix timestamps
-for moments and intervals ([b7dcbaf](https://github.com/xymaxim/ytpb/commit/
-b7dcbaf6eebe3f6022b7fa8eefe98f4b8af7c4cb)) - Add `ytpb.playback.RewindTreeMap`
-to keep rewind history ([91fd078](https://github.com/xymaxim/ytpb/commit/
-91fd078caf37f31fee167e0c2a20a38aa2badcd8)) ### Breaking changes - Rename
-`ytpb.mpd` to `ytpb.representations` - Rename `ytpb.exceptions` to
-`ytpb.errors` - Rename `ytpb.playback.Playback.get_downloaded_segment` to
-`ytpb.playback.Playback.get_segment` - Rename
-`ytpb.representations.extract_representations_info` to
-`ytpb.representations.extract_representations` - Remove unused
-`ytpb.representations.strip_manifest` ## [2024.3.27] - Add Containerfile with
-instructions to build patched FFmpeg and MPV ### Breaking changes - Change
-return value of `ytpb.locate.SegmentLocator.find_sequence_by_time` to
-`ytpb.locate.LocateResult` ## [2024.3.16] - Add options to dump base (`--dump-
-base-urls`) and segment (`--dump-segment-urls`) URLs to the `download` command
-([#10](https://github.com/xymaxim/ytpb/pull/10)) - Add the [Cookbook](https://
-ytpb.readthedocs.io/en/latest/cookbook.html) documentation page ## [2024.3.13]
-- Add the config.toml.example file - Add ability to use [custom aliases](https:
-//ytpb.readthedocs.io/en/latest/reference.html#custom-aliases) in format specs
-- Add [aliases](https://ytpb.readthedocs.io/en/latest/reference.html#itags) for
-itags (`@`) as [dynamic aliases](https://ytpb.readthedocs.io/en/latest/
-reference.html#aliases) - Fix allowing empty representations in the CLI
-commands ## [2024.3.9] - Add the CHANGELOG file and documentation page - Change
-the first segment locating step: don\'t limit it to two jumps ([#8](https://
-github.com/xymaxim/ytpb/pull/8)) [2024.5.12]: https://github.com/xymaxim/ytpb/
-compare/v2024.5.3..v2024.5.12 [2024.5.3]: https://github.com/xymaxim/ytpb/
-compare/v2024.4.20..v2024.5.3 [2024.4.20]: https://github.com/xymaxim/ytpb/
-compare/v2024.4.12..v2024.4.20 [2024.4.12]: https://github.com/xymaxim/ytpb/
-compare/v2024.3.27..v2024.4.12 [2024.3.27]: https://github.com/xymaxim/ytpb/
-compare/v2024.3.16..v2024.3.27 [2024.3.16]: https://github.com/xymaxim/ytpb/
-compare/v2024.3.13..v2024.3.16 [2024.3.13]: https://github.com/xymaxim/ytpb/
-compare/v2024.3.9..v2024.3.13 [2024.3.9]: https://github.com/xymaxim/ytpb/
-compare/v2024.3.7..v2024.3.9
+Changelog ######### Versions follow `Calendar Versioning`_ with the
+``YYYY.M.D`` scheme. .. _Calendar Versioning: https://calver.org `2024.5.3`_
+*********** - Add support for resumable downloads (`#13
+github.com/xymaxim/ytpb/pull/13>`__) - Change the segments output directory
+from the run temporary directory to a directory under the current working one -
+Add ``--ignore-resume``, ``-S / --keep-segments``, and ``--segments-output-
+dir`` options - Change the default output path to ``
+_`` - Rename the ``--no-cleanup`` option to ``--keep-temp`` - Replace the ``--
+preview`` option with ``--preview-start`` and ``--preview-end`` `2024.4.20`_
+************ - Fix wrong frame rate values of the video-only merged files when
+boundary segments are cut and encoded with H.264 (`e1120bf
+github.com/xymaxim/ytpb/commit/e1120bf4514333ff3ac5d4eac862ccb6a9d5f606>`__) -
+Write metadata tags with basic and rewind information to merged files (`aa7adf1
+github.com/xymaxim/ytpb/commit/aa7adf1580e5a83c9abaa76f2836b9a0570cc4ba>`__) -
+Add the ``--no-metadata`` option to not write metadata tags to merged files
+`2024.4.12`_ ************ - Add the `Python package
+ytpb.readthedocs.io/en/latest/package/index.html>`__ page with the basic usage
+and API reference - Add the ``--version`` CLI option to show version number -
+Add :attr:`ytpb.representations.RepresentationInfo.type` property - Add :attr:
+`ytpb.playback.RewindInterval.duration` and :attr:
+`~ytpb.playback.RewindInterval.sequences` properties - Accept Unix timestamps
+for moments and intervals (`b7dcbaf
+github.com/xymaxim/ytpb/commit/b7dcbaf6eebe3f6022b7fa8eefe98f4b8af7c4cb>`__) -
+Add :class:`ytpb.playback.RewindTreeMap` to keep rewind history (`91fd078
+github.com/xymaxim/ytpb/commit/91fd078caf37f31fee167e0c2a20a38aa2badcd8>`__)
+Breaking changes ================ - Rename :mod:`ytpb.mpd` to :mod:
+`ytpb.representations` - Rename :mod:`ytpb.exceptions` to :mod:`ytpb.errors` -
+Rename :meth:`ytpb.playback.Playback.get_downloaded_segment` to :meth:
+`~ytpb.playback.Playback.get_segment` - Rename :meth:
+`ytpb.representations.extract_representations_info` to :meth:
+`~ytpb.representations.extract_representations` - Remove unused :meth:
+`ytpb.representations.strip_manifest` `2024.3.27`_ ************ - Add
+Containerfile with instructions to build patched FFmpeg and MPV Breaking
+changes ================ - Change return value of :meth:
+`ytpb.locate.SegmentLocator.find_sequence_by_time` to :class:
+`~ytpb.locate.LocateResult` `2024.3.16`_ ************ - Add options to dump
+base (``--dump-base-urls``) and segment (``--dump-segment-urls``) URLs to the
+``download`` command (`#10
+github.com/xymaxim/ytpb/pull/10>`__) - Add the `Cookbook`_ documentation page
+.. _Cookbook: https://ytpb.readthedocs.io/en/latest/cookbook.html `2024.3.13`_
+************ - Add the config.toml.example file - Add ability to use `custom
+aliases`_ in format specs - Add `aliases`_ for itags (``@``) as `dynamic
+aliases`_ - Fix allowing empty representations in the CLI commands .. _custom
+aliases: https://ytpb.readthedocs.io/en/latest/reference.html#custom-aliases ..
+_aliases: https://ytpb.readthedocs.io/en/latest/reference.html#itags ..
+_dynamic aliases: https://ytpb.readthedocs.io/en/latest/reference.html#aliases
+`2024.3.9`_ *********** - Add the CHANGELOG file and documentation page -
+Change the first segment locating step: don't limit it to two jumps (`#8
+github.com/xymaxim/ytpb/pull/8>`__) .. _2024.5.3: https://github.com/xymaxim/
+ytpb/compare/v2024.4.20..v2024.5.3 .. _2024.4.20: https://github.com/xymaxim/
+ytpb/compare/v2024.4.12..v2024.4.20 .. _2024.4.12: https://github.com/xymaxim/
+ytpb/compare/v2024.3.27..v2024.4.12 .. _2024.3.27: https://github.com/xymaxim/
+ytpb/compare/v2024.3.16..v2024.3.27 .. _2024.3.16: https://github.com/xymaxim/
+ytpb/compare/v2024.3.13..v2024.3.16 .. _2024.3.13: https://github.com/xymaxim/
+ytpb/compare/v2024.3.9..v2024.3.13 .. _2024.3.9: https://github.com/xymaxim/
+ytpb/compare/v2024.3.7..v2024.3.9
```

### Comparing `ytpb-2024.5.12/CONTRIBUTING.rst` & `ytpb-2024.5.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/config.toml.example` & `ytpb-2024.5.3/config.toml.example`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/docs/cli.rst` & `ytpb-2024.5.3/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/docs/cookbook.rst` & `ytpb-2024.5.3/docs/cookbook.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/docs/quick.rst` & `ytpb-2024.5.3/docs/quick.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/docs/reference.rst` & `ytpb-2024.5.3/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/docs/why.rst` & `ytpb-2024.5.3/docs/why.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/docs/package/index.rst` & `ytpb-2024.5.3/docs/package/index.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/docs/package/usage.rst` & `ytpb-2024.5.3/docs/package/usage.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/etc/Containerfile` & `ytpb-2024.5.3/etc/Containerfile`

 * *Files 14% similar despite different names*

```diff
@@ -10,27 +10,25 @@
 
 RUN apk --no-cache add build-base git coreutils autoconf automake cmake \
   nasm yasm meson ninja-build libtool ffmpeg-dev mpv-dev libxxhash libdovi \
   libunwind-dev libplacebo-dev glslang-dev elfutils-dev mesa-dev \
   freetype-dev fribidi harfbuzz-dev mujs lua5.2-dev luajit rubberband uchardet \
   alsa-lib jack libpulse libvpx-dev x264-dev gnutls-dev xrandr
 
-# See https://github.com/mpv-player/mpv-build/pull/203.
 RUN ln -sf /usr/lib/ninja-build/bin/ninja /usr/bin/ninja
 
 WORKDIR ${BUILDDIR}
 RUN git clone https://github.com/mpv-player/mpv-build .
 
 RUN ./update
 
 WORKDIR ${BUILDDIR}/ffmpeg
-COPY *.patch .
 RUN <<EOF
-git apply 0001-Revert-http-Send-a-Range-header-even-when-the-offset.patch
-git apply 0002-Revert-http-Improve-handling-of-Content-Range-with-T.patch
+git revert --no-commit c122831
+git revert --no-commit 0dd1ff6
 EOF
 
 WORKDIR ${BUILDDIR}
 RUN printf "%s\n" --enable-gnutls --enable-libx264 --enable-libvpx \
   --enable-libxml2 --enable-demuxer=dash > ffmpeg_options
 
 # Stage 2. Build FFmpeg and mpv.
```

### Comparing `ytpb-2024.5.12/src/ytpb/api.py` & `ytpb-2024.5.3/src/ytpb/api.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/cache.py` & `ytpb-2024.5.3/src/ytpb/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             path.unlink()
 
         if _check_item_is_expired(latest_item_path.name):
             logger.debug("Found expired cached item: %s", latest_item_path)
             latest_item_path.unlink()
             item = None
         else:
-            with open(latest_item_path, encoding="utf-8") as f:
+            with open(latest_item_path) as f:
                 item = json.load(f)
             logger.debug("Found unexpired cached item: %s", latest_item_path)
 
     return item
 
 
 def write_to_cache(
@@ -71,15 +71,15 @@
         cache_directory: A cached items location.
     """
     cache_directory.mkdir(parents=True, exist_ok=True)
     if old_item_paths := _find_cached_item_paths(key, cache_directory):
         for path in old_item_paths:
             path.unlink()
     new_item_path = cache_directory / f"{expires_at}~{key}"
-    with open(new_item_path, "w", encoding="utf-8") as f:
+    with open(new_item_path, "w") as f:
         json.dump(item, f)
     logger.debug("New cache item has been created: %s", new_item_path)
 
 
 def remove_expired_cache_items(cache_directory: Path) -> None:
     """Removes expired cache items."""
     for path in sorted(cache_directory.glob("*~*")):
```

### Comparing `ytpb-2024.5.12/src/ytpb/conditional.py` & `ytpb-2024.5.3/src/ytpb/conditional.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/config.py` & `ytpb-2024.5.3/src/ytpb/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
 
 def setup_logging(level: int) -> None:
     structlog.configure(
         processors=[
             structlog.processors.add_log_level,
             structlog.processors.StackInfoRenderer(),
-            structlog.processors.TimeStamper(fmt="iso", utc=True),
+            structlog.processors.TimeStamper(fmt="%s.%f", utc=True),
             structlog.dev.ConsoleRenderer(
                 exception_formatter=structlog.dev.plain_traceback,
                 # For details about NO_COLOR, see https://no-color.org/
                 colors="NO_COLOR" not in os.environ,
             ),
             structlog.dev.set_exc_info,
         ],
```

### Comparing `ytpb-2024.5.12/src/ytpb/download.py` & `ytpb-2024.5.3/src/ytpb/download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/errors.py` & `ytpb-2024.5.3/src/ytpb/errors.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/fetchers.py` & `ytpb-2024.5.3/src/ytpb/fetchers.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/info.py` & `ytpb-2024.5.3/src/ytpb/info.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/locate.py` & `ytpb-2024.5.3/src/ytpb/locate.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/merge.py` & `ytpb-2024.5.3/src/ytpb/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 
 import functools
 import os
 import shlex
 from pathlib import Path
 from typing import Any
 
-import av
-
-from ytpb.utils import ffmpeg
+from ytpb import ffmpeg
 
 __all__ = ("merge_segments", "mux_and_cut_boundary_segment")
 
 
 DEFAULT_VIDEO_ENCODING_SETTINGS = {
     "h264": "libx264 -crf 18",
     "vp9": "libvpx-vp9 -crf 31 -b:v 0",
@@ -63,17 +61,17 @@
 
     if not {"cut_at_start", "cut_at_end"} > cut_kwargs.keys():
         raise ValueError(
             "only cut_at_start or cut_at_end keyword argument is accepted in cut_kwargs"
         )
 
     if video_segment_path and video_codec is None:
-        with av.open(video_segment_path) as container:
-            video_av_stream = container.streams.get({"video": 0})[0]
-            video_codec = video_av_stream.codec_context.name
+        video_codec = ffmpeg.ffprobe_show_entries(
+            video_segment_path, "stream=codec_name"
+        )
 
     ffmpeg_input_options = []
     ffmpeg_codecs_options = []
 
     should_cut = bool(
         cut_kwargs.get("cut_at_start", 0) or cut_kwargs.get("cut_at_end", 0)
     )
@@ -97,15 +95,15 @@
             else:
                 try:
                     ffmpeg_codecs_options += ["-c:v"] + shlex.split(
                         DEFAULT_VIDEO_ENCODING_SETTINGS[video_codec]
                     )
                 except KeyError:
                     raise ValueError(
-                        "No encoding settings are availabe for "
+                        "No encoding settings are availabe for"
                         f"'{video_codec}' video codec"
                     )
 
         if audio_segment_path:
             ffmpeg_input_options += prepare_ffmpeg_input_options(
                 audio_segment_path, **cut_kwargs
             )
@@ -243,17 +241,17 @@
         start_video_segment_path = get_nth_or_none(video_segment_paths, 0)
 
         end_audio_segment_path = get_nth_or_none(audio_segment_paths, -1)
         end_video_segment_path = get_nth_or_none(video_segment_paths, -1)
 
         video_codec: str | None = None
         if video_segment_paths:
-            with av.open(video_segment_paths[0]) as container:
-                video_av_stream = container.streams.get({"video": 0})[0]
-                video_codec = video_av_stream.codec_context.name
+            video_codec = ffmpeg.ffprobe_show_entries(
+                video_segment_paths[0], "stream=codec_name"
+            )
 
         if num_of_segments == 1:
             segment_trimmed_path = Path(temp_directory, "a.a" + output_extension)
             mux_and_cut_boundary_segment(
                 start_audio_segment_path,
                 start_video_segment_path,
                 segment_trimmed_path,
```

### Comparing `ytpb-2024.5.12/src/ytpb/playback.py` & `ytpb-2024.5.3/src/ytpb/playback.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
     @classmethod
     def from_manifest(
         cls,
         manifest_path: Path,
         fetch_video_info: bool = True,
         **kwargs,
     ) -> "Playback":
-        with open(manifest_path, "r", encoding="utf-8") as f:
+        with open(manifest_path, "r") as f:
             list_of_streams = extract_representations(f.read())
             streams = Streams(list_of_streams)
 
         some_base_url = next(iter(streams)).base_url
         video_url = build_video_url_from_base_url(some_base_url)
 
         if not check_base_url_is_expired(some_base_url):
```

### Comparing `ytpb-2024.5.12/src/ytpb/representations.py` & `ytpb-2024.5.3/src/ytpb/representations.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/segment.py` & `ytpb-2024.5.3/src/ytpb/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,11 +145,14 @@
                 name_as_key = name.removesuffix("-Us").lower().replace("-", "_")
                 parsed_metadata_fields[name_as_key] = value
 
         return SegmentMetadata(**parsed_metadata_fields)
 
     def get_actual_duration(self) -> float:
         """Gets the actual segment duration in seconds."""
-        with av.open(self.local_path) as container:
+        with av.open(str(self.local_path)) as container:
             first_packet, *_, last_packet = list(container.demux())[:-1]
-        end_pts = last_packet.pts + last_packet.duration
-        return float((end_pts - first_packet.pts) * first_packet.time_base)
+            end_timestamp = last_packet.pts + last_packet.duration
+            duration = (end_timestamp - first_packet.pts) * float(
+                first_packet.time_base
+            )
+            return duration
```

### Comparing `ytpb-2024.5.12/src/ytpb/streams.py` & `ytpb-2024.5.3/src/ytpb/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,23 +98,22 @@
     ) -> list[AudioOrVideoStream]:
         """Queries streams by a format spec.
 
         Notes:
             Check for attributes is strict. This means that the following code
             will fail with :class:`.QueryError` because audio streams don't have
             the ``height`` attribute::
-
-                audio_streams.query("height eq 1080")
+              audio_streams.query("height eq 1080")
 
         Examples:
             Query streams of a specific media format using aliases::
 
-                playback.streams.query(
-                    "@webm", aliases={"webm": "format eq webm"}
-                )
+              playback.streams.query(
+                  "@webm", aliases={"webm": "format eq webm"}
+              )
 
         References:
             https://ytpb.readthedocs.io/en/latest/reference.html#format-spec
 
         Args:
             format_spec: A format spec. May contains aliases.
             aliases: A dictionary of aliases.
```

### Comparing `ytpb-2024.5.12/src/ytpb/types.py` & `ytpb-2024.5.3/src/ytpb/types.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/actions/capture.py` & `ytpb-2024.5.3/src/ytpb/actions/capture.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/actions/compose.py` & `ytpb-2024.5.3/src/ytpb/actions/compose.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/actions/download.py` & `ytpb-2024.5.3/src/ytpb/actions/download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/cli/__init__.py` & `ytpb-2024.5.3/src/ytpb/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from typing import Any, cast, TextIO
 
 import click
 import cloup
 import structlog
 import toml
 
-from ytpb._version import __version__
 from ytpb.cli.commands.capture import capture_group
 from ytpb.cli.commands.download import download_command
 from ytpb.cli.commands.mpd import mpd_group
 
 from ytpb.cli.common import suppress_output
 from ytpb.cli.options import config_options, logging_options
 from ytpb.config import (
@@ -92,15 +91,15 @@
         "--quiet",
         help="Supress all normal output.",
         default=False,
         is_flag=True,
         is_eager=True,
     ),
 )
-@click.version_option(__version__, "-V", "--version", message="%(version)s")
+@click.version_option(None, "-V", "--version", message="%(version)s")
 @click.pass_context
 def base_cli(
     ctx: click.Context,
     config_path: Path,
     no_config: bool,
     debug: bool,
     report: bool,
@@ -117,27 +116,26 @@
         suppress_output()
 
     if report:
         debug = True
         os.environ["NO_COLOR"] = "1"
 
         timestamp = datetime.now(tz=timezone.utc).strftime("%Y%m%d-%H%M%S")
-        report_file_path = Path.cwd() / f"ytpb-{timestamp}.log"
-        report_handle = open(report_file_path, "a", encoding="utf-8")
+        report_handle = open(Path.cwd() / f"ytpb-{timestamp}.log", "a")
         sys.stdout = cast(
             TextIO, ReportStreamWrapper(ctx.obj.original_stdout, report_handle)
         )
         sys.stderr = cast(TextIO, ReportStreamWrapper(sys.stderr, report_handle))
 
         @atexit.register
         def sanitize_report_file() -> None:
             report_handle.close()
             with FileInput(report_handle.name, inplace=True) as fi:
                 for line in fi:
-                    print(re.sub(r"/ip/([\w.:]+)/", "/ip/0.0.0.0/", line), end="")
+                    print(re.sub("/ip/([\w.:]+)/", "/ip/0.0.0.0/", line), end="")
 
     setup_logging(logging.DEBUG if debug else logging.WARNING)
 
     if not no_config:
         if config_path:
             logger.info("Using configuration from '%s' via --config", config_path)
             load_config_into_context(ctx, config_path)
```

### Comparing `ytpb-2024.5.12/src/ytpb/cli/common.py` & `ytpb-2024.5.3/src/ytpb/cli/common.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/cli/options.py` & `ytpb-2024.5.3/src/ytpb/cli/options.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/cli/parameters.py` & `ytpb-2024.5.3/src/ytpb/cli/parameters.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/cli/commands/capture.py` & `ytpb-2024.5.3/src/ytpb/cli/commands/capture.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/cli/commands/download.py` & `ytpb-2024.5.3/src/ytpb/cli/commands/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,16 +400,16 @@
     actual_date_interval = DateInterval(
         start_segment.ingestion_start_date,
         end_segment.ingestion_end_date,
     )
 
     cut_kwargs: dict[str, float] = {}
     if not no_cut:
-        cut_at_start = 0 if preview_start else rewind_interval.start.cut_at
-        cut_at_end = 0 if preview_end else rewind_interval.end.cut_at
+        cut_at_start = rewind_interval.start.cut_at if preview_start else 0
+        cut_at_end = rewind_interval.end.cut_at if preview_end else 0
         cut_kwargs.update(
             {
                 "cut_at_start": cut_at_start,
                 "cut_at_end": cut_at_end,
             }
         )
         actual_date_interval = DateInterval(
```

### Comparing `ytpb-2024.5.12/src/ytpb/cli/commands/mpd.py` & `ytpb-2024.5.3/src/ytpb/cli/commands/mpd.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         final_output_path = output_path
     final_output_path = resolve_output_path(final_output_path)
 
     click.echo("(<<) Composing MPEG-DASH manifest...")
     streams = Streams(queried_audio_streams + queried_video_streams)
     composed_manifest = compose_static_mpd(playback, rewind_interval, streams)
 
-    with open(final_output_path, "w", encoding="utf-8") as f:
+    with open(final_output_path, "w") as f:
         f.write(composed_manifest)
 
     try:
         saved_to_path_value = f"{final_output_path.relative_to(Path.cwd())}"
     except ValueError:
         saved_to_path_value = final_output_path
 
@@ -292,15 +292,15 @@
     except BroadcastStatusError as e:
         match e.status:
             case BroadcastStatus.COMPLETED:
                 click.echo("Stream was live, but now it's finished", err=True)
         sys.exit(1)
 
     refreshed = refresh_mpd(manifest_content, playback.streams)
-    with open(manifest, "w", encoding="utf-8") as f:
+    with open(manifest, "w") as f:
         f.write(refreshed)
 
     some_base_url = next(iter(playback.streams)).base_url
     expires_at_time = int(extract_parameter_from_url("expire", some_base_url))
     expires_at_date = datetime.fromtimestamp(expires_at_time)
     expires_in = express_timedelta_in_words(expires_at_date - datetime.now())
```

### Comparing `ytpb-2024.5.12/src/ytpb/utils/date.py` & `ytpb-2024.5.3/src/ytpb/utils/date.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import enum
 import math
-import os
 import re
 import string
 import warnings
 from dataclasses import dataclass
 from datetime import datetime, time, timedelta
 from typing import Any, Literal
 
@@ -103,23 +102,20 @@
     IN_SENTENCE = "[%-H h ][%-M m ][%-S s]"
 
 
 def format_duration(duration: timedelta, pattern: DurationFormatPattern) -> str:
     total_seconds = math.floor(duration.total_seconds() + 0.5)
     total_minutes, ss = divmod(total_seconds, 60)
     hh, mm = divmod(total_minutes, 60)
+
+    output = pattern.value
     time_object = time(hh, mm, ss)
 
-    pattern_value = pattern.value
-    if os.name == "nt":
-        pattern_value = pattern_value.replace("%-", "%#")
-
-    output = pattern_value
-    optional_parts_re = r"\[(?P<part>(?P<fmt>%[-#]?[HMS]).*?)\]"
-    for matched in re.finditer(optional_parts_re, pattern_value):
+    optional_parts_re = r"\[(?P<part>(?P<fmt>%-?[HMS]).*?)\]"
+    for matched in re.finditer(optional_parts_re, pattern.value):
         if int(time_object.strftime(matched.group("fmt"))) == 0:
             output = output.replace(matched.group(0), "")
         else:
             formatted_part = time_object.strftime(matched.group("part"))
             output = output.replace(matched.group(0), formatted_part)
 
     output = time_object.strftime(output).rstrip(" ")
```

### Comparing `ytpb-2024.5.12/src/ytpb/utils/other.py` & `ytpb-2024.5.3/src/ytpb/utils/other.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/utils/path.py` & `ytpb-2024.5.3/src/ytpb/utils/path.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/utils/remote.py` & `ytpb-2024.5.3/src/ytpb/utils/remote.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/src/ytpb/utils/url.py` & `ytpb-2024.5.3/src/ytpb/utils/url.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/conftest.py` & `ytpb-2024.5.3/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,17 +67,15 @@
 ) -> None:
     test_cache_directory = Path(os.environ["XDG_CACHE_HOME"]) / "ytpb"
     test_cache_directory.mkdir(parents=True)
 
     some_base_url = streams_in_list[0].base_url
     expired_at = int(some_base_url.split("/expire/")[1].split("/")[0])
 
-    with open(
-        test_cache_directory / f"{expired_at}~{video_id}", "w", encoding="utf-8"
-    ) as f:
+    with open(test_cache_directory / f"{expired_at}~{video_id}", "w") as f:
         test_cached_item = {
             "info": asdict(active_live_video_info),
             "streams": [asdict(stream) for stream in streams_in_list],
         }
         json.dump(test_cached_item, f)
 
 
@@ -210,15 +208,15 @@
 @pytest.fixture()
 def video_base_url() -> str:
     return "https://rr5---sn-25ge7nzr.googlevideo.com/videoplayback/expire/1695928670/ei/_nwVZYXhAqbQvdIPjKmqgAM/ip/0.0.0.0/id/kHwmzef842g.2/itag/244/source/yt_live_broadcast/requiressl/yes/spc/UWF9fy2D4rPPhPMeyQnmxgP0Yhyaohs/vprv/1/playlist_type/DVR/ratebypass/yes/mime/video%2Fwebm/live/1/gir/yes/noclen/1/dur/2.000/keepalive/yes/fexp/24007246/beids/24350017/sparams/expire,ei,ip,id,itag,source,requiressl,spc,vprv,playlist_type,ratebypass,mime,live,gir,noclen,dur/sig/AOq0QJ8wRgIhAJBYRElUjO7WhY5_gsjtj0aUbXbyb9Z_Yjo7JeecnqrzAiEAkzwV4SYIFponf7BddjJ5hscSZr8hbPBSx09Qffev9AA%3D/initcwndbps/623750/mh/XB/mm/44/mn/sn-25ge7nzr/ms/lva/mt/1695906793/mv/m/mvi/5/pl/38/lsparams/initcwndbps,mh,mm,mn,ms,mv,mvi,pl/lsig/AG3C_xAwRQIhAP_FmY_xO0cSx-hk2oibYFE1AHaCvDHeYyMXXUEuBNeVAiARmaf6MprHE-eEJJx3Ai59WyTOSt8INUUWhA7MSoEO2w%3D%3D/"
 
 
 @pytest.fixture()
 def youtube_dl_info() -> dict:
-    with open(TEST_DATA_PATH / "info-1695928670.json", encoding="utf-8") as f:
+    with open(TEST_DATA_PATH / "info-1695928670.json") as f:
         return json.load(f)
 
 
 @pytest.fixture()
 def streams_in_list(youtube_dl_info: dict) -> list[AudioOrVideoStream]:
     list_of_streams: list[AudioOrVideoStream] = []
     for f in youtube_dl_info["formats"]:
```

### Comparing `ytpb-2024.5.12/tests/helpers.py` & `ytpb-2024.5.3/tests/helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from datetime import timezone
 from pathlib import Path
 
-import av
 import pytest
 
+from ytpb.ffmpeg import ffprobe_show_entries
 
-def assert_number_of_streams(file_path: Path, expected: int):
-    with av.open(file_path) as container:
-        assert len(container.streams) == expected
 
+def assert_number_of_streams(filepath: Path, expected: int):
+    assert ffprobe_show_entries(filepath, "format=nb_streams") == str(expected)
 
-def assert_approx_duration(file_path: Path, expected: float, abs: float = 2.2e-2):
-    with av.open(file_path) as container:
-        actual = container.duration / 1e6
 
+def assert_approx_duration(filepath: Path, expected: float, abs: float = 2.2e-2):
+    actual = float(ffprobe_show_entries(filepath, "format=duration"))
     approx_expected = pytest.approx(expected, abs=abs)
     if actual != approx_expected:
         raise AssertionError(
             "Durations are not almost equal\n"
             f" - expected: {approx_expected}\n"
             f" + actual: {actual}"
         )
```

### Comparing `ytpb-2024.5.12/tests/test_cache.py` & `ytpb-2024.5.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/test_download.py` & `ytpb-2024.5.3/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/test_fetchers.py` & `ytpb-2024.5.3/tests/test_fetchers.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/test_locate.py` & `ytpb-2024.5.3/tests/test_locate.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def read_gap_case_fixture_data(path: Path) -> dict:
     class Row(NamedTuple):
         sequence: str
         ingestion_walltime_ms: str
         duration_s: str
 
     data = {}
-    with open(path, encoding="utf-8") as f:
+    with open(path) as f:
         reader = csv.reader(f, delimiter=",")
         next(reader)
         for fields in reader:
             row = Row(*fields)
             data[int(row.sequence)] = (
                 float(row.ingestion_walltime_ms) / 1e6,
                 float(row.duration_s),
```

### Comparing `ytpb-2024.5.12/tests/test_merge.py` & `ytpb-2024.5.3/tests/test_merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 from pathlib import Path
 
-import av
 import pytest
 
 from conftest import TEST_DATA_PATH
-from helpers import assert_approx_duration, assert_number_of_streams
 
+from helpers import assert_approx_duration, assert_number_of_streams
 from ytpb.merge import merge_segments
 
 SEGMENT_BASE_PATH = Path(TEST_DATA_PATH) / "segments"
 
 
 def setup_function():
     os.environ["YTPB_VP9_ENCODING_SETTINGS"] = (
```

### Comparing `ytpb-2024.5.12/tests/test_playback.py` & `ytpb-2024.5.3/tests/test_playback.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,21 +296,19 @@
     streams_in_list: list[AudioOrVideoStream],
     video_id: str,
     stream_url: str,
     tmp_path: Path,
 ):
     # Given:
     test_cache_directory = Playback.get_cache_directory()
-    test_cache_directory.mkdir(parents=True, exist_ok=True)
+    test_cache_directory.mkdir(parents=True)
 
     frozen_time = datetime.fromisoformat("2123-09-28T17:00:00+00:00").timestamp()
     expired_at = int(frozen_time - 10)
-    with open(
-        test_cache_directory / f"{expired_at}~{video_id}", "w", encoding="utf-8"
-    ) as f:
+    with open(test_cache_directory / f"{expired_at}~{video_id}", "w") as f:
         test_cache = {
             "info": asdict(active_live_video_info),
             "streams": [asdict(stream) for stream in streams_in_list],
         }
         json.dump(test_cache, f)
 
     # When:
```

### Comparing `ytpb-2024.5.12/tests/test_playback_session.py` & `ytpb-2024.5.3/tests/test_playback_session.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/test_representations.py` & `ytpb-2024.5.3/tests/test_representations.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/test_segment.py` & `ytpb-2024.5.3/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/test_streams.py` & `ytpb-2024.5.3/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/test_types.py` & `ytpb-2024.5.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/actions/test_compose.py` & `ytpb-2024.5.3/tests/actions/test_compose.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/actions/test_download.py` & `ytpb-2024.5.3/tests/actions/test_download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/cli/conftest.py` & `ytpb-2024.5.3/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/cli/test_download_command.py` & `ytpb-2024.5.3/tests/cli/test_download_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import glob
 import os
 import pickle
-import platform
 import re
 import shutil
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Callable
 from unittest.mock import MagicMock, patch
 from urllib.parse import urljoin
 
-import av
 import click
 import pytest
 import responses
 import toml
 
 from conftest import TEST_DATA_PATH
 from freezegun import freeze_time
 from helpers import assert_approx_duration
 
 from ytpb.config import DEFAULT_CONFIG
+from ytpb.ffmpeg import ffprobe_show_entries
 from ytpb.playback import RewindInterval, RewindMoment
 
 
 @pytest.mark.parametrize(
     "interval,output_subpath",
     [
         # Segments and corresponding ingestion start dates:
@@ -37,15 +36,14 @@
         ("2023-03-25T23:33:55+00/2023-03-25T23:33:57+00", "233355+00.mp4"),
         ("2023-03-25T23:33:55+00/PT3S", "233355+00.mp4"),
         ("2023-03-25T23:33:55+00/7959121", "233355+00.mp4"),
         ("PT3S/7959121", "233355+00.mp4"),
         ("PT3S/2023-03-25T23:33:58+00", "233355+00.mp4"),
     ],
 )
-@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_download_within_interval(
     interval: str,
     output_subpath: str,
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
@@ -78,16 +76,16 @@
                 stream_url,
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
 
     # Then:
-    assert result.exit_code == 0
     assert result.output == expected_out
+    assert result.exit_code == 0
     assert glob.glob(str(tmp_path / f"*{output_subpath}"))
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_providing_start_and_end_equals_now(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
@@ -344,15 +342,14 @@
     assert os.path.exists(run_temp_directory / "7959121.i140.mp4")
 
 
 @pytest.mark.parametrize(
     "audio_format,video_format",
     [("itag eq 140", "itag eq 244"), ("itag eq 140", "none"), ("none", "itag eq 244")],
 )
-@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_download_audio_and_or_video(
     audio_format: str | None,
     video_format: str | None,
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
@@ -569,15 +566,14 @@
     assert result.exit_code == 0
     assert os.path.exists(
         tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4"
     )
     assert os.path.exists(run_temp_directory / "7959120.i140.mp4")
 
 
-@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_no_merge_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
@@ -609,22 +605,21 @@
                 "--no-merge",
                 stream_url,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
-    assert expected_out == result.output
     assert not os.path.exists(
         tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4"
     )
     assert not os.path.exists(run_temp_directory)
+    assert expected_out == result.output
 
 
-@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_dry_run_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
@@ -663,15 +658,14 @@
     assert result.output == expected_out
     assert not os.path.exists(
         tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4"
     )
     assert not os.path.exists(run_temp_directory)
 
 
-@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_no_cut_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
@@ -703,19 +697,20 @@
                 "--no-cut",
                 stream_url,
             ],
         )
 
     # Then:
     assert result.exit_code == 0
-    assert result.output == expected_out
     expected_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4"
     assert os.path.exists(expected_path)
     assert_approx_duration(expected_path, 4.0)
 
+    assert result.output == expected_out
+
 
 @freeze_time("2023-09-28T17:00:00+00:00")
 def test_from_cache(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     create_cache_file: None,
@@ -907,15 +902,15 @@
             "download": {
                 "audio_format": "NON-SENS",
             }
         }
     }
     config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
     config_path.parent.mkdir(parents=True)
-    with config_path.open("w", encoding="utf-8") as f:
+    with config_path.open("w") as f:
         toml.dump(config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
@@ -958,26 +953,26 @@
             "download": {
                 "audio_format": "NON-SENS",
             }
         }
     }
     default_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
     default_config_path.parent.mkdir(parents=True)
-    with default_config_path.open("w", encoding="utf-8") as f:
+    with default_config_path.open("w") as f:
         toml.dump(default_config, f)
 
     test_config = {
         "options": {
             "download": {
                 "audio_format": "itag eq 140",
             }
         }
     }
     test_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "test-config.toml"
-    with test_config_path.open("w", encoding="utf-8") as f:
+    with test_config_path.open("w") as f:
         toml.dump(test_config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
@@ -1011,22 +1006,22 @@
     default_config = {
         "options": {
             "download": {
                 "audio_format": "NON-SENS",
             }
         }
     }
-    default_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb" / "config.toml"
+    default_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
     default_config_path.parent.mkdir(parents=True)
-    with default_config_path.open("w", encoding="utf-8") as f:
+    with default_config_path.open("w") as f:
         toml.dump(default_config, f)
 
-    test_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb" / "test-config.toml"
+    test_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "test-config.toml"
 
-    # Then:
+    # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         with pytest.raises(click.FileError) as exc_info:
             ytpb_cli_invoke(
                 [
                     "--config",
                     test_config_path,
@@ -1038,14 +1033,16 @@
                     "none",
                     stream_url,
                 ],
                 catch_exceptions=False,
                 standalone_mode=False,
             )
 
+    assert str(test_config_path) in str(exc_info)
+
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_no_config_option(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
@@ -1066,15 +1063,15 @@
             "download": {
                 "interval": "7959120/7959121",
             }
         }
     }
     default_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
     default_config_path.parent.mkdir(parents=True)
-    with default_config_path.open("w", encoding="utf-8") as f:
+    with default_config_path.open("w") as f:
         toml.dump(default_config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         with pytest.raises(click.MissingParameter) as exc_info:
             ytpb_cli_invoke(
@@ -1113,15 +1110,15 @@
             "download": {
                 "audio_format": "NON-SENS",
             }
         }
     }
     default_config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
     default_config_path.parent.mkdir(parents=True)
-    with default_config_path.open("w", encoding="utf-8") as f:
+    with default_config_path.open("w") as f:
         toml.dump(default_config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         with pytest.raises(click.UsageError) as exc_info:
             ytpb_cli_invoke(
@@ -1227,15 +1224,15 @@
             "aliases": {
                 "custom-alias": "itag eq 140",
             }
         }
     }
     config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
     config_path.parent.mkdir(parents=True)
-    with config_path.open("w", encoding="utf-8") as f:
+    with config_path.open("w") as f:
         toml.dump(custom_config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
@@ -1498,14 +1495,15 @@
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     audio_base_url: str,
     tmp_path: Path,
+    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1526,38 +1524,40 @@
                 stream_url,
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
 
     # Then:
-    output_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4"
-    with av.open(output_path) as container:
-        metadata_tags = container.metadata
-
-    assert metadata_tags["title"] == "Webcam Zürich HB"
-    assert metadata_tags["author"] == "David Gubler"
-    assert metadata_tags["comment"] == stream_url
-    assert metadata_tags["input_start_time"] == "1679787235.000000"
-    assert metadata_tags["input_end_time"] == "1679787237.000000"
-    assert metadata_tags["actual_start_time"] == "1679787235.000000"
-    assert metadata_tags["actual_end_time"] == "1679787237.000000"
-    assert metadata_tags["start_sequence_number"] == "7959120"
-    assert metadata_tags["end_sequence_number"] == "7959121"
+    format_tags = ffprobe_show_entries(
+        tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4",
+        "format_tags",
+        "default",
+    )
+    assert "TAG:title=Webcam Zürich HB" in format_tags
+    assert "TAG:author=David Gubler" in format_tags
+    assert f"TAG:comment={stream_url}" in format_tags
+    assert "TAG:input_start_time=1679787235.000000" in format_tags
+    assert "TAG:input_end_time=1679787237.000000" in format_tags
+    assert "TAG:actual_start_time=1679787235.000000" in format_tags
+    assert "TAG:actual_end_time=1679787237.000000" in format_tags
+    assert "TAG:start_sequence_number=7959120" in format_tags
+    assert "TAG:end_sequence_number=7959121" in format_tags
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_metadata_tags_without_cutting(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     audio_base_url: str,
     tmp_path: Path,
+    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1579,39 +1579,41 @@
                 stream_url,
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
 
     # Then:
-    output_path = tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4"
-    with av.open(output_path) as container:
-        metadata_tags = container.metadata
-
-    assert metadata_tags["title"] == "Webcam Zürich HB"
-    assert metadata_tags["author"] == "David Gubler"
-    assert metadata_tags["comment"] == stream_url
-    assert metadata_tags["input_start_time"] == "1679787235.000000"
-    assert metadata_tags["input_end_time"] == "1679787237.000000"
-    assert metadata_tags["actual_start_time"] == "1679787234.491176"
-    assert metadata_tags["actual_end_time"] == "1679787238.486826"
-    assert metadata_tags["start_sequence_number"] == "7959120"
-    assert metadata_tags["end_sequence_number"] == "7959121"
+    format_tags = ffprobe_show_entries(
+        tmp_path / "Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4",
+        "format_tags",
+        "default",
+    )
+    assert "TAG:title=Webcam Zürich HB" in format_tags
+    assert "TAG:author=David Gubler" in format_tags
+    assert f"TAG:comment={stream_url}" in format_tags
+    assert "TAG:input_start_time=1679787235.000000" in format_tags
+    assert "TAG:input_end_time=1679787237.000000" in format_tags
+    assert "TAG:actual_start_time=1679787234.491176" in format_tags
+    assert "TAG:actual_end_time=1679787238.486826" in format_tags
+    assert "TAG:start_sequence_number=7959120" in format_tags
+    assert "TAG:end_sequence_number=7959121" in format_tags
 
 
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_resume_downloading(
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
+    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1684,14 +1686,15 @@
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
+    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1730,14 +1733,15 @@
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
+    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1776,14 +1780,15 @@
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
+    expected_out,
 ) -> None:
     # Given:
     sub_tmp_path = tmp_path / "sub"
     sub_tmp_path.mkdir()
     monkeypatch.chdir(sub_tmp_path)
 
     segments_output_directory = sub_tmp_path / segments_output_dir_option
@@ -1829,14 +1834,15 @@
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
+    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1877,14 +1883,15 @@
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
+    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1926,14 +1933,15 @@
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
+    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
 
@@ -1969,14 +1977,15 @@
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     mocked_responses: responses.RequestsMock,
     fake_info_fetcher: MagicMock,
     video_id: str,
     audio_base_url: str,
     tmp_path: Path,
+    expected_out,
 ) -> None:
     # Given:
     add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"),
     )
```

### Comparing `ytpb-2024.5.12/tests/cli/test_parameters.py` & `ytpb-2024.5.3/tests/cli/test_parameters.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/cli/capture/test_frame_command.py` & `ytpb-2024.5.3/tests/cli/capture/test_frame_command.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/cli/mpd/test_compose_command.py` & `ytpb-2024.5.3/tests/cli/mpd/test_compose_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import os
-import platform
 from pathlib import Path
 from typing import Callable
 from unittest.mock import MagicMock, patch
 from urllib.parse import urljoin
 
 import pytest
+
 import toml
 from freezegun import freeze_time
 
 
 @pytest.mark.parametrize(
     "audio_formats,video_formats",
     [
         ("itag eq 140", "itag eq 243 or itag eq 244"),
         ("itag eq 140", "none"),
         ("none", "itag eq 243 or itag eq 244"),
     ],
 )
-@pytest.mark.expect_suffix(platform.system())
 def test_compose_mpd(
     audio_formats,
     video_formats,
     ytpb_cli_invoke: Callable,
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     fake_info_fetcher: MagicMock,
@@ -50,15 +49,14 @@
                 stream_url,
             ],
         )
     assert result.exit_code == 0
     assert result.output == expected_out
 
 
-@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-03-26T00:00:00+00:00")
 def test_compose_mpd_with_no_streams(
     ytpb_cli_invoke: Callable,
     fake_info_fetcher: MagicMock,
     stream_url: str,
     video_id: str,
     audio_base_url: str,
@@ -145,15 +143,15 @@
                     "audio_formats": "NON-SENS",
                 }
             }
         }
     }
     config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
     config_path.parent.mkdir(parents=True)
-    with config_path.open("w", encoding="utf-8") as f:
+    with config_path.open("w") as f:
         toml.dump(config, f)
 
     # When:
     with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
         mock_fetcher.return_value = fake_info_fetcher
         result = ytpb_cli_invoke(
             [
```

### Comparing `ytpb-2024.5.12/tests/cli/mpd/test_refresh_command.py` & `ytpb-2024.5.3/tests/cli/mpd/test_refresh_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # ruff: noqa: E501
 
 import copy
-import platform
 from dataclasses import asdict
 from difflib import unified_diff
 from pathlib import Path
 from typing import Callable
 from unittest.mock import MagicMock, patch
 
 import freezegun
@@ -42,15 +41,14 @@
       </Representation>
     </AdaptationSet>
   </Period>
 </MPD>
 """
 
 
-@pytest.mark.expect_suffix(platform.system())
 @freeze_time("2023-08-16T02:30:00+02:00", tz_offset=2)
 def test_refresh_mpd(
     ytpb_cli_invoke: Callable,
     mock_fetch_and_set_essential: MagicMock,
     streams_in_list: list[AudioOrVideoStream],
     active_live_video_info: YouTubeVideoInfo,
     stream_url: str,
@@ -59,15 +57,15 @@
     video_base_url: str,
     dash_manifest: str,
     tmp_path: Path,
     expected_out,
 ) -> None:
     # Given:
     manifest_path = tmp_path / "manifest.mpd"
-    with open(manifest_path, "w", encoding="utf-8") as f:
+    with open(manifest_path, "w") as f:
         f.write(dash_manifest)
 
     # When:
     def mock_essential(obj: Playback, *args, **kwargs):
         updated_streams = copy.deepcopy(streams_in_list)
         for i, stream in enumerate(updated_streams):
             stream_as_dict = asdict(stream)
@@ -84,15 +82,15 @@
     ):
         result = ytpb_cli_invoke(["mpd", "refresh", str(manifest_path)])
 
     # Then:
     assert result.exit_code == 0
     assert result.output == expected_out
 
-    with open(manifest_path, encoding="utf-8") as f:
+    with open(manifest_path) as f:
         refreshed_manifest = f.read()
 
     actual_diff = list(
         unified_diff(
             dash_manifest.splitlines(keepends=True),
             refreshed_manifest.splitlines(keepends=True),
             n=0,
```

### Comparing `ytpb-2024.5.12/tests/data/info-1695928670.json` & `ytpb-2024.5.3/tests/data/info-1695928670.json`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/manifest-1695928670.mpd` & `ytpb-2024.5.3/tests/data/manifest-1695928670.mpd`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/webpage-1695928670.html` & `ytpb-2024.5.3/tests/data/webpage-1695928670.html`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244]-Darwin.out` & `ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244]-Linux.out` & `ytpb-2024.5.3/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
-These 3 representations will be in the manifest:
-                          (Audio)                           
-    itag    | Format        | Codec         | Sampling      
-------------|---------------|---------------|---------------
-    140     | mp4           | mp4a.40.2     | 44100 Hz      
+These 2 representations will be in the manifest:
                           (Video)                           
     itag    | Format        | Codec         | Quality       
 ------------|---------------|---------------|---------------
     243     | webm          | vp9           | 360p          
     244     | webm          | vp9           | 480p          
 
 (<<) Locating start and end in the stream... done.
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244]-Windows.out` & `ytpb-2024.5.3/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-Run playback for https://www.youtube.com/watch?v=kHwmzef842g
-(<<) Collecting info about the video...
-Stream 'Webcam Zürich HB' is alive!
-These 3 representations will be in the manifest:
-                          (Audio)                           
-    itag    | Format        | Codec         | Sampling      
-------------|---------------|---------------|---------------
-    140     | mp4           | mp4a.40.2     | 44100 Hz      
-                          (Video)                           
-    itag    | Format        | Codec         | Quality       
-------------|---------------|---------------|---------------
-    243     | webm          | vp9           | 360p          
-    244     | webm          | vp9           | 480p          
-
-(<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
-
-(<<) Composing MPEG-DASH manifest...
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mpd'.
-~ Note that the manifest will expire in 6 hours.
+Run playback for https://www.youtube.com/watch?v=kHwmzef842g
+(<<) Collecting info about the video...
+Stream 'Webcam Zürich HB' is alive!
+This representation will be in the manifest:
+                          (Audio)                           
+    itag    | Format        | Codec         | Sampling      
+------------|---------------|---------------|---------------
+    140     | mp4           | mp4a.40.2     | 44100 Hz      
+
+(<<) Locating start and end in the stream... done.
+Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
+  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
+
+(<<) Composing MPEG-DASH manifest...
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mpd'.
+~ Note that the manifest will expire in 6 hours.
```

#### encoding

```diff
@@ -1 +1 @@
-iso-8859-1
+utf-8
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244]-Darwin.out` & `ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244]-Linux.out` & `ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
-These representations will be downloaded:
+This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
-   - Video: itag 244, webm (vp9), 854x480, 30 fps
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-   - Video ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (no cut requested)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mkv'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none]-Darwin.out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out`

 * *Files 6% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-2. Merging segments (no cut requested)... done.
+2. Merging segments (may take a while)... done.
 
 Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none]-Linux.out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
+  Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-2. Merging segments (no cut requested)... done.
+2. Merging segments (may take a while)... done.
 
 Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none]-Windows.out` & `ytpb-2024.5.3/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Run playback for https://www.youtube.com/watch?v=kHwmzef842g
-(<<) Collecting info about the video...
-Stream 'Webcam Zürich HB' is alive!
-This representation will be downloaded:
-   - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
-
-(<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
-
-(<<) Preparing and saving the excerpt...
-1. Downloading segments 7959120-7959121:
-   - Audio ---------------------------- 2/2 100% eta 0:00:00
-2. Merging segments (no cut requested)... done.
-
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
+Run playback for https://www.youtube.com/watch?v=kHwmzef842g
+(<<) Collecting info about the video...
+Stream 'Webcam Zürich HB' is alive!
+This representation will be downloaded:
+   - Video: itag 244, webm (vp9), 854x480, 30 fps
+
+(<<) Locating start and end in the stream... done.
+Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
+  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
+
+(<<) Preparing and saving the excerpt...
+1. Downloading segments 7959120-7959121:
+   - Video ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
+2. Merging segments (no cut requested)... done.
+
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.webm'.
```

#### encoding

```diff
@@ -1 +1 @@
-iso-8859-1
+utf-8
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244]-Darwin.out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
-   - Video: itag 244, webm (vp9), 854x480, 30 fps
+   - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
+Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
-   - Video ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-2. Merging segments (no cut requested)... done.
+   - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
+2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.webm'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244]-Linux.out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
-   - Video: itag 244, webm (vp9), 854x480, 30 fps
+   - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
+Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
-   - Video ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-2. Merging segments (no cut requested)... done.
+   - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
+2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.webm'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244]-Windows.out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Run playback for https://www.youtube.com/watch?v=kHwmzef842g
-(<<) Collecting info about the video...
-Stream 'Webcam Zürich HB' is alive!
-This representation will be downloaded:
-   - Video: itag 244, webm (vp9), 854x480, 30 fps
-
-(<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
-
-(<<) Preparing and saving the excerpt...
-1. Downloading segments 7959120-7959121:
-   - Video ---------------------------- 2/2 100% eta 0:00:00
-2. Merging segments (no cut requested)... done.
-
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.webm'.
+Run playback for https://www.youtube.com/watch?v=kHwmzef842g
+(<<) Collecting info about the video...
+Stream 'Webcam Zürich HB' is alive!
+This representation will be downloaded:
+   - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
+
+(<<) Locating start and end in the stream... done.
+Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
+  Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
+
+(<<) Preparing and saving the excerpt...
+1. Downloading segments 7959120-7959121:
+   - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
+2. Merging segments (may take a while)... done.
+
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

#### encoding

```diff
@@ -1 +1 @@
-iso-8859-1
+utf-8
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4]-Darwin.out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
+  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
 Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4]-Linux.out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
 Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
+  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
 Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4]-Darwin.out` & `ytpb-2024.5.3/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
-  Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
+Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
+  Actual end: 25 Mar 2023 23:33:57 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
 2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
+Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00.mp4'.
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4]-Linux.out` & `ytpb-2024.5.3/tests/data/expected/test_no_cut_option.out`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
+Actual start: 25 Mar 2023 23:33:54 +0000 (-00:01), seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
 (<<) Preparing and saving the excerpt...
 1. Downloading segments 7959120-7959121:
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-2. Merging segments (may take a while)... done.
+2. Merging segments (no cut requested)... done.
 
 Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
```

### Comparing `ytpb-2024.5.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4]-Darwin.out` & `ytpb-2024.5.3/tests/data/expected/test_no_merge_option.out`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Run playback for https://www.youtube.com/watch?v=kHwmzef842g
 (<<) Collecting info about the video...
 Stream 'Webcam Zürich HB' is alive!
 This representation will be downloaded:
    - Audio: itag 140, mp4 (mp4a.40.2), 44100 Hz
 
 (<<) Locating start and end in the stream... done.
-Actual start: 25 Mar 2023 23:33:55 +0000, seq. 7959120
+Actual start: 25 Mar 2023 23:33:54 +0000, seq. 7959120
   Actual end: 25 Mar 2023 23:33:58 +0000, seq. 7959121
 
-(<<) Preparing and saving the excerpt...
-1. Downloading segments 7959120-7959121:
+(<<) Downloading segments 7959120-7959121 (no merge requested)...
    - Audio ━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2/2 100% eta 0:00:00
-2. Merging segments (may take a while)... done.
 
-Success! Saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233355+00.mp4'.
+Success! Segments saved to 'Webcam-Zurich-HB_kHwmzef842g_20230325T233354+00'.
```

### Comparing `ytpb-2024.5.12/tests/data/gap-cases/gap-case-1-fixture.csv` & `ytpb-2024.5.3/tests/data/gap-cases/gap-case-1-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/gap-cases/gap-case-2-fixture.csv` & `ytpb-2024.5.3/tests/data/gap-cases/gap-case-2-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/gap-cases/gap-case-3-fixture.csv` & `ytpb-2024.5.3/tests/data/gap-cases/gap-case-3-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/segments/7959120.i140.mp4` & `ytpb-2024.5.3/tests/data/segments/7959120.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/segments/7959120.i244.webm` & `ytpb-2024.5.3/tests/data/segments/7959120.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/segments/7959121.i140.mp4` & `ytpb-2024.5.3/tests/data/segments/7959121.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/segments/7959121.i244.webm` & `ytpb-2024.5.3/tests/data/segments/7959121.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/segments/7959122.i140.mp4` & `ytpb-2024.5.3/tests/data/segments/7959122.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/segments/7959122.i244.webm` & `ytpb-2024.5.3/tests/data/segments/7959122.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/segments/7959123.i140.mp4` & `ytpb-2024.5.3/tests/data/segments/7959123.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/segments/7959123.i244.webm` & `ytpb-2024.5.3/tests/data/segments/7959123.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/segments/7959203.i140.mp4` & `ytpb-2024.5.3/tests/data/segments/7959203.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/data/segments/7959203.i244.webm` & `ytpb-2024.5.3/tests/data/segments/7959203.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/utils/test_date.py` & `ytpb-2024.5.3/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/utils/test_path.py` & `ytpb-2024.5.3/tests/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/utils/test_remote.py` & `ytpb-2024.5.3/tests/utils/test_remote.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/tests/utils/test_url.py` & `ytpb-2024.5.3/tests/utils/test_url.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/.gitignore` & `ytpb-2024.5.3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 notebooks/shared/*
 !notebooks/shared/.gitkeep
 notebooks/out/
 
-src/ytpb/_version.py
-
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `ytpb-2024.5.12/LICENSE` & `ytpb-2024.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ytpb-2024.5.12/README.rst` & `ytpb-2024.5.3/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -58,40 +58,23 @@
   <https://asciinema.org/a/653865>`__)
 - Creating a time-lapse of a live stream excerpt (`link
   <https://asciinema.org/a/653869>`__)
 
 Installation
 ************
 
-Ytpb requires Python 3.11 or higher and has been `tested
-<https://github.com/xymaxim/ytpb/actions/workflows/ci.yml>`__ on Linux, macOS,
-and Windows. Also, it needs the recent version of `FFmpeg
-<https://ffmpeg.org/download.html>`__ to be installed.
-
-Installing from PyPI
-====================
-
-When you have all required dependencies, you can install Ytpb via `pipx
+Ytpb requires Python 3.11 or higher. The recommended way is to use `pipx
 <https://pypa.github.io/pipx/>`_::
 
   $ pipx install ytpb
 
 To upgrade to the newer version, do::
 
   $ pipx upgrade ytpb
 
-Windows binaries
-================
-
-For Windows, pre-built binaries are available: check `releases
-<https://github.com/xymaxim/ytpb/releases>`__ on GitHub. Make sure to `add
-<https://www.wikihow.com/Install-FFmpeg-on-Windows>`__ the ``ffmpeg.exe`` file
-to your system path or place it in the folder next to the Ytpb binary. Now
-you're ready to use Ytpb in Terminal: type commands, not double-click.
-
 Further reading
 ***************
 
 After installing, check out the `documentation`_. The `Why Ytpb?`_ page explains
 why the project exists. For main usage scenarios, see `Quick start`_. The
 `Command line application`_ page goes deeper into the usage. `Reference`_
 provides some general aspects and terms. `Cookbook`_ contains some useful
```

### Comparing `ytpb-2024.5.12/pyproject.toml` & `ytpb-2024.5.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [ "hatchling", "hatch-vcs" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "ytpb"
 description = "A playback for YouTube live streams"
 readme = "README.rst"
-dynamic = ["version"]
+version = "2024.5.3"
 authors = [ { name = "Maxim Stolyarchuk" } ]
 keywords = [ "youtube" ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
@@ -48,42 +48,31 @@
 dev = [
     "ytpb[test]",
     "pre-commit",
 ]
 docs = [
     "sphinx==7.2.6",
     "sphinx-toolbox==3.5.0",
-    "myst-parser==3.0.1",
 ]
 
 [project.urls]
 Source = "https://github.com/xymaxim/ytpb"
 Documentation = "https://ytpb.readthedocs.io"
 
 [project.scripts]
 ytpb = "ytpb.__main__:main"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
-[tool.hatch.version]
-source = "vcs"
-
-[tool.hatch.version.raw-options]
-version_scheme = "calver-by-date"
-local_scheme = "dirty-tag"
-
-[tool.hatch.build.hooks.vcs]
-version-file = "src/ytpb/_version.py"
-
 [tool.hatch.build.targets.sdist]
 exclude = [
    "/.github",
    "/notebooks",
 ]
 
 [tool.black]
 line-length = 88
 
 [tool.pytest.ini_options]
 pm-patterns-base-dir = "tests/data/expected/"
-pm-pattern-file-fmt = "{fn}{callspec}{suffix}"
+pm-pattern-file-fmt = "{fn}{callspec}"
```

### Comparing `ytpb-2024.5.12/PKG-INFO` & `ytpb-2024.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ytpb
-Version: 2024.5.12
+Version: 2024.5.3
 Summary: A playback for YouTube live streams
 Project-URL: Source, https://github.com/xymaxim/ytpb
 Project-URL: Documentation, https://ytpb.readthedocs.io
 Author: Maxim Stolyarchuk
 License: MIT License
         
         Copyright (c) 2024 Maxim Stolyarchuk
@@ -54,15 +54,14 @@
 Requires-Dist: freezegun>=1.4.0; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest-matcher==2.0.1; extra == 'dev'
 Requires-Dist: pytest-socket>=0.6.0; extra == 'dev'
 Requires-Dist: pytest>=7.4.4; extra == 'dev'
 Requires-Dist: responses>=0.24.1; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: myst-parser==3.0.1; extra == 'docs'
 Requires-Dist: sphinx-toolbox==3.5.0; extra == 'docs'
 Requires-Dist: sphinx==7.2.6; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: freezegun>=1.4.0; extra == 'test'
 Requires-Dist: pytest-matcher==2.0.1; extra == 'test'
 Requires-Dist: pytest-socket>=0.6.0; extra == 'test'
 Requires-Dist: pytest>=7.4.4; extra == 'test'
@@ -129,40 +128,23 @@
   <https://asciinema.org/a/653865>`__)
 - Creating a time-lapse of a live stream excerpt (`link
   <https://asciinema.org/a/653869>`__)
 
 Installation
 ************
 
-Ytpb requires Python 3.11 or higher and has been `tested
-<https://github.com/xymaxim/ytpb/actions/workflows/ci.yml>`__ on Linux, macOS,
-and Windows. Also, it needs the recent version of `FFmpeg
-<https://ffmpeg.org/download.html>`__ to be installed.
-
-Installing from PyPI
-====================
-
-When you have all required dependencies, you can install Ytpb via `pipx
+Ytpb requires Python 3.11 or higher. The recommended way is to use `pipx
 <https://pypa.github.io/pipx/>`_::
 
   $ pipx install ytpb
 
 To upgrade to the newer version, do::
 
   $ pipx upgrade ytpb
 
-Windows binaries
-================
-
-For Windows, pre-built binaries are available: check `releases
-<https://github.com/xymaxim/ytpb/releases>`__ on GitHub. Make sure to `add
-<https://www.wikihow.com/Install-FFmpeg-on-Windows>`__ the ``ffmpeg.exe`` file
-to your system path or place it in the folder next to the Ytpb binary. Now
-you're ready to use Ytpb in Terminal: type commands, not double-click.
-
 Further reading
 ***************
 
 After installing, check out the `documentation`_. The `Why Ytpb?`_ page explains
 why the project exists. For main usage scenarios, see `Quick start`_. The
 `Command line application`_ page goes deeper into the usage. `Reference`_
 provides some general aspects and terms. `Cookbook`_ contains some useful
```

