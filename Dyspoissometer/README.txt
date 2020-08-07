These are TARGA images which can be manipulated by KolourPaint for Linux and other image editing utilities. As a hacker, all you really need to know is this, which is true of most but not all TGA files:

1. The header is 0x12 (18) bytes long.

2. There is no footer.

3. The pixels are 3 bytes each: blue, green, red. They start immediately after the header.

4. Offset 0xC of the header contains the 16-bit pixel width in little endian.

5. Offset 0xE of the header contains the 16-bit pixel height in little endian.

Note that sample.7z was compressed with 7Zip. It will uncompress to sample.tga .
