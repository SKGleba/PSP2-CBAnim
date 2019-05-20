# PSP2-CBAnim
BootAnimation creator for enso_ex and CBS-Manager
# Usage
"cbanim -intype filename%d [optional flags]"
 - intype: input file type [ -r: raw | -g: gif | -p: png/jpg]. Note: there is also a resize parameter "s" (screen res) or "l" (lanimation), it can be used with -g/-p (-sg/-sp), if set, cbanim will resize the input data to 960x544 or 960x128 (the file remains untouched).
 - filename%d: the base file name where the %d is instead of the frame number (e.g frame_%d.bin for frame_0.bin, frame_1.bin, ..)
 - noloop: the animation will be played once
 - nocompress: the animation will not be compressed (very slow, not recommended)
 - nopreload: the animation will not be loaded to ram, but directly read from the img file
 - slowmode: animation will be slower, but it wont have possible artifacts
 
example: "./cbanim -g anim.gif -noloop"
# Notes:
 - You need ImageMagick and gzip (or convert.exe and gzip.exe) to use this tool.
