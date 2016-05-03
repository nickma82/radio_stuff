David's Radio Stuff
===================

This repository contains small Radio and SDR related utilities.

*   converters/dat_to_vcd.c

    Convert a bit stream to .VCD for processing in GTKWave

*   converters/am_to_ook.c

    Convert output of rtl_fm's AM demodulation to binary stream

*   converters/pack_bit_stream.c

    Convert 1-bit per byte stream to packed bit stream

*   decoders/decode_somfy.c

    Decode Somfy RTS from a demodulated bitstream

Usage Example:

 rtl_fm -M am -f 433.42M -s 270K | ./am_to_ook -d 10 -t 2000 -  | ./decode_somfy
