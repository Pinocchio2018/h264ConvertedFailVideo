# h264ConvertedFailVideo


## fail case
ffmpeg convert command
```
ffmpeg -i ./060322_010.h264  output-fail.mp4
```

console output 
```
...... omit some output
[h264 @ 0x5569b3fd4c40] If you want to help, upload a sample of this file to https://streams.videolan.org/upload/ and contact the ffmpeg-devel mailing list. (ffmpeg-devel@ffmpeg.org)
[h264 @ 0x5569b3fd4c40] no frame!
Error while decoding stream #0:0: Invalid data found when processing input
[h264 @ 0x5569b40a3f00] data partitioning is not implemented. Update your FFmpeg version to the newest one from Git. If the problem still occurs, it means that your file has a feature which has not been implemented.
[h264 @ 0x5569b40a3f00] If you want to help, upload a sample of this file to https://streams.videolan.org/upload/ and contact the ffmpeg-devel mailing list. (ffmpeg-devel@ffmpeg.org)
[h264 @ 0x5569b40a3f00] no frame!
Error while decoding stream #0:0: Invalid data found when processing input
[h264 @ 0x5569b399e900] data partitioning is not implemented. Update your FFmpeg version to the newest one from Git. If the problem still occurs, it means that your file has a feature which has not been implemented.
[h264 @ 0x5569b399e900] If you want to help, upload a sample of this file to https://streams.videolan.org/upload/ and contact the ffmpeg-devel mailing list. (ffmpeg-devel@ffmpeg.org)
[h264 @ 0x5569b399e900] no frame!
Error while decoding stream #0:0: Invalid data found when processing input
[h264 @ 0x5569b3a73cc0] data partitioning is not implemented. Update your FFmpeg version to the newest one from Git. If the problem still occurs, it means that your file has a feature which has not been implemented.
[h264 @ 0x5569b3a73cc0] If you want to help, upload a sample of this file to https://streams.videolan.org/upload/ and contact the ffmpeg-devel mailing list. (ffmpeg-devel@ffmpeg.org)
[h264 @ 0x5569b3a73cc0] no frame!
Error while decoding stream #0:0: Invalid data found when processing input
[h264 @ 0x5569b3a966c0] data partitioning is not implemented. Update your FFmpeg version to the newest one from Git. If the problem still occurs, it means that your file has a feature which has not been implemented.
[h264 @ 0x5569b3a966c0] If you want to help, upload a sample of this file to https://streams.videolan.org/upload/ and contact the ffmpeg-devel mailing list. (ffmpeg-devel@ffmpeg.org)
[h264 @ 0x5569b3a966c0] no frame!
Error while decoding stream #0:0: Invalid data found when processing input
[h264 @ 0x5569b3e36a40] data partitioning is not implemented. Update your FFmpeg version to the newest one from Git. If the problem still occurs, it means that your file has a feature which has not been implemented.
[h264 @ 0x5569b3e36a40] If you want to help, upload a sample of this file to https://streams.videolan.org/upload/ and contact the ffmpeg-devel mailing list. (ffmpeg-devel@ffmpeg.org)
[h264 @ 0x5569b3e36a40] no frame!
Error while decoding stream #0:0: Invalid data found when processing input
[h264 @ 0x5569b3f05b40] data partitioning is not implemented. Update your FFmpeg version to the newest one from Git. If the problem still occurs, it means that your file has a feature which has not been implemented.
[h264 @ 0x5569b3f05b40] If you want to help, upload a sample of this file to https://streams.videolan.org/upload/ and contact the ffmpeg-devel mailing list. (ffmpeg-devel@ffmpeg.org)
[h264 @ 0x5569b3f05b40] no frame!
Error while decoding stream #0:0: Invalid data found when processing input
[h264 @ 0x5569b3fd4c40] data partitioning is not implemented. Update your FFmpeg version to the newest one from Git. If the problem still occurs, it means that your file has a feature which has not been implemented.
[h264 @ 0x5569b3fd4c40] If you want to help, upload a sample of this file to https://streams.videolan.org/upload/ and contact the ffmpeg-devel mailing list. (ffmpeg-devel@ffmpeg.org)
[h264 @ 0x5569b3fd4c40] no frame!
Error while decoding stream #0:0: Invalid data found when processing input
    Last message repeated 5 times
Cannot determine format of input stream 0:0 after EOF
Error marking filters as finished
Conversion failed!

```

## success case
ffmpeg convert command
```
ffmpeg -i ./064647_100.h264  output-success.mp4  
```
console output
```
ffmpeg version n5.1.2 Copyright (c) 2000-2022 the FFmpeg developers
  built with gcc 12.2.0 (GCC)
  configuration: --prefix=/usr --disable-debug --disable-static --disable-stripping --enable-amf --enable-avisynth --enable-cuda-llvm --enable-lto --enable-fontconfig --enable-gmp --enable-gnutls --enable-gpl --enable-ladspa --enable-libaom --enable-libass --enable-libbluray --enable-libbs2b --enable-libdav1d --enable-libdrm --enable-libfreetype --enable-libfribidi --enable-libgsm --enable-libiec61883 --enable-libjack --enable-libmfx --enable-libmodplug --enable-libmp3lame --enable-libopencore_amrnb --enable-libopencore_amrwb --enable-libopenjpeg --enable-libopus --enable-libpulse --enable-librav1e --enable-librsvg --enable-libsoxr --enable-libspeex --enable-libsrt --enable-libssh --enable-libsvtav1 --enable-libtheora --enable-libv4l2 --enable-libvidstab --enable-libvmaf --enable-libvorbis --enable-libvpx --enable-libwebp --enable-libx264 --enable-libx265 --enable-libxcb --enable-libxml2 --enable-libxvid --enable-libzimg --enable-nvdec --enable-nvenc --enable-opencl --enable-opengl --enable-shared --enable-version3 --enable-vulkan
  libavutil      57. 28.100 / 57. 28.100
  libavcodec     59. 37.100 / 59. 37.100
  libavformat    59. 27.100 / 59. 27.100
  libavdevice    59.  7.100 / 59.  7.100
  libavfilter     8. 44.100 /  8. 44.100
  libswscale      6.  7.100 /  6.  7.100
  libswresample   4.  7.100 /  4.  7.100
  libpostproc    56.  6.100 / 56.  6.100
[hevc @ 0x5603bdd83840] Invalid NAL unit 11, skipping.
Input #0, hevc, from './064647_100.h264':
  Duration: N/A, bitrate: N/A
  Stream #0:0: Video: hevc (Main), yuv420p(tv, bt709), 2304x1296, 15 fps, 15 tbr, 1200k tbn
File 'output-success.mp4' already exists. Overwrite? [y/N] y
Stream mapping:
  Stream #0:0 -> #0:0 (hevc (native) -> h264 (libx264))
Press [q] to stop, [?] for help
[libx264 @ 0x5603bdd9f4c0] using cpu capabilities: MMX2 SSE2Fast SSSE3 SSE4.2 AVX FMA3 BMI2 AVX2
[libx264 @ 0x5603bdd9f4c0] profile High, level 5.0, 4:2:0, 8-bit
[libx264 @ 0x5603bdd9f4c0] 264 - core 164 r3095 baee400 - H.264/MPEG-4 AVC codec - Copyleft 2003-2022 - http://www.videolan.org/x264.html - options: cabac=1 ref=3 deblock=1:0:0 analyse=0x3:0x113 me=hex subme=7 psy=1 psy_rd=1.00:0.00 mixed_ref=1 me_range=16 chroma_me=1 trellis=1 8x8dct=1 cqm=0 deadzone=21,11 fast_pskip=1 chroma_qp_offset=-2 threads=9 lookahead_threads=1 sliced_threads=0 nr=0 decimate=1 interlaced=0 bluray_compat=0 constrained_intra=0 bframes=3 b_pyramid=2 b_adapt=1 b_bias=0 direct=1 weightb=1 open_gop=0 weightp=2 keyint=250 keyint_min=15 scenecut=40 intra_refresh=0 rc_lookahead=40 rc=crf mbtree=1 crf=23.0 qcomp=0.60 qpmin=0 qpmax=69 qpstep=4 ip_ratio=1.40 aq=1:1.00
Output #0, mp4, to 'output-success.mp4':
  Metadata:
    encoder         : Lavf59.27.100
  Stream #0:0: Video: h264 (avc1 / 0x31637661), yuv420p(tv, bt709, progressive), 2304x1296, q=2-31, 15 fps, 15360 tbn
    Metadata:
      encoder         : Lavc59.37.100 libx264
    Side data:
      cpb: bitrate max/min/avg: 0/0/0 buffer size: 0 vbv_delay: N/A
[hevc @ 0x5603bde0fd00] Invalid NAL unit 11, skipping.0.00 bitrate=N/A speed=   0x    
[NULL @ 0x5603bdd83840] Invalid NAL unit 29, skipping.05.66 bitrate=3700.9kbits/s speed=1.71x     
[hevc @ 0x5603bde0fd00] Invalid NAL unit 29, skipping.
[NULL @ 0x5603bdd83840] Invalid NAL unit 5, skipping.:19.53 bitrate=2469.4kbits/s speed=2.63x    
[hevc @ 0x5603bde0fd00] Invalid NAL unit 5, skipping.
[NULL @ 0x5603bdd83840] Invalid NAL unit 29, skipping.20.86 bitrate=2412.1kbits/s speed=2.63x    
[hevc @ 0x5603bde38780] Invalid NAL unit 29, skipping.
[NULL @ 0x5603bdd83840] Invalid NAL unit 11, skipping.29.20 bitrate=2082.8kbits/s speed=2.89x    
[hevc @ 0x5603bdda02c0] Invalid NAL unit 11, skipping.
[NULL @ 0x5603bdd83840] Invalid NAL unit 14, skipping.32.93 bitrate=2037.7kbits/s speed=2.95x    
[hevc @ 0x5603bde00a00] Invalid NAL unit 14, skipping.
[NULL @ 0x5603bdd83840] Invalid NAL unit 30, skipping.39.80 bitrate=2213.1kbits/s speed=2.88x    
[hevc @ 0x5603bde00a00] Invalid NAL unit 30, skipping.
[NULL @ 0x5603bdd83840] Invalid NAL unit 30, skipping.56.40 bitrate=2937.5kbits/s speed=2.39x    
[hevc @ 0x5603be40fe40] Invalid NAL unit 30, skipping.
[NULL @ 0x5603bdd83840] Invalid NAL unit 9, skipping.:06.20 bitrate=2977.8kbits/s speed=2.39x    
[hevc @ 0x5603bde0fd00] Invalid NAL unit 9, skipping.
frame= 1078 fps= 35 q=-1.0 Lsize=   27849kB time=00:01:11.66 bitrate=3183.3kbits/s speed=2.31x    
video:27836kB audio:0kB subtitle:0kB other streams:0kB global headers:0kB muxing overhead: 0.044874%
[libx264 @ 0x5603bdd9f4c0] frame I:5     Avg QP:16.54  size:328439
[libx264 @ 0x5603bdd9f4c0] frame P:475   Avg QP:19.72  size: 44494
[libx264 @ 0x5603bdd9f4c0] frame B:598   Avg QP:24.20  size:  9577
[libx264 @ 0x5603bdd9f4c0] consecutive B-frames: 19.8% 15.8%  9.2% 55.3%
[libx264 @ 0x5603bdd9f4c0] mb I  I16..4:  4.9% 73.4% 21.6%
[libx264 @ 0x5603bdd9f4c0] mb P  I16..4:  2.2%  9.3%  1.1%  P16..4: 25.1%  7.8%  4.5%  0.0%  0.0%    skip:49.9%
[libx264 @ 0x5603bdd9f4c0] mb B  I16..4:  0.4%  1.0%  0.1%  B16..8: 24.6%  2.3%  0.6%  direct: 1.7%  skip:69.3%  L0:47.4% L1:49.0% BI: 3.5%
[libx264 @ 0x5603bdd9f4c0] 8x8 transform intra:72.9% inter:80.0%
[libx264 @ 0x5603bdd9f4c0] coded y,uvDC,uvAC intra: 54.9% 51.7% 19.1% inter: 9.7% 7.5% 0.3%
[libx264 @ 0x5603bdd9f4c0] i16 v,h,dc,p: 30% 24%  8% 37%
[libx264 @ 0x5603bdd9f4c0] i8 v,h,dc,ddl,ddr,vr,hd,vl,hu: 30% 18% 16%  5%  5% 10%  4%  6%  6%
[libx264 @ 0x5603bdd9f4c0] i4 v,h,dc,ddl,ddr,vr,hd,vl,hu: 36% 17% 12%  4%  8% 12%  4%  4%  3%
[libx264 @ 0x5603bdd9f4c0] i8c dc,h,v,p: 49% 21% 24%  6%
[libx264 @ 0x5603bdd9f4c0] Weighted P-Frames: Y:0.0% UV:0.0%
[libx264 @ 0x5603bdd9f4c0] ref P L0: 72.7% 15.9%  8.7%  2.7%
[libx264 @ 0x5603bdd9f4c0] ref B L0: 92.4%  6.8%  0.8%
[libx264 @ 0x5603bdd9f4c0] ref B L1: 97.0%  3.0%
[libx264 @ 0x5603bdd9f4c0] kb/s:3172.97

```
