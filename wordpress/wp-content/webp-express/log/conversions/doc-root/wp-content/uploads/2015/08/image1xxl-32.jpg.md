WebP Express 0.15.3. Conversion triggered using bulk conversion, 2019-09-24 04:56:23

*WebP Convert 2.1.4*  ignited.
- PHP version: 7.3.1
- Server software: Apache

Stack converter ignited

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2015/08/image1xxl-32.jpg
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image1xxl-32.jpg.webp
- log-call-arguments: true
- converters: (array of 9 items)

The following options have not been explicitly set, so using the following defaults:
- converter-options: (empty array)
- shuffle: false
- preferred-converters: (empty array)
- extra-converters: (empty array)

The following options were supplied and are passed on to the converters in the stack:
- default-quality: 70
- encoding: "auto"
- max-quality: 80
- metadata: "none"
- near-lossless: 60
- quality: "auto"
------------


*Trying: cwebp* 

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2015/08/image1xxl-32.jpg
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image1xxl-32.jpg.webp
- default-quality: 70
- encoding: "auto"
- low-memory: true
- log-call-arguments: true
- max-quality: 80
- metadata: "none"
- method: 6
- near-lossless: 60
- quality: "auto"
- use-nice: true
- command-line-options: ""
- try-common-system-paths: true
- try-supplied-binary-for-os: true

The following options have not been explicitly set, so using the following defaults:
- alpha-quality: 85
- auto-filter: false
- preset: "none"
- size-in-percentage: null (not set)
- skip: false
- rel-path-to-precompiled-binaries: *****
------------

Encoding is set to auto - converting to both lossless and lossy and selecting the smallest file

Converting to lossy
Locating cwebp binaries
1 cwebp binaries found in common system locations
Checking if we have a supplied binary for OS: Darwin... We do.
We in fact have 1
A total of 2 cwebp binaries where found
Detecting versions of the cwebp binaries found (and verifying that they can be executed in the process)
Executing: /usr/local/bin/cwebp -version. Result: version: 1.0.3
Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12 -version
Exec failed (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12)
Trying executing the cwebs found until success. Starting with the ones with highest version number.
Creating command line options for version: 1.0.3
Quality of source is 83. This is higher than max-quality, so using max-quality instead (80)
The near-lossless option ignored for lossy
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 80 -alpha_q '85' -m 6 -low_memory '[doc-root]/wp-content/uploads/2015/08/image1xxl-32.jpg' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image1xxl-32.jpg.webp.lossy.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image1xxl-32.jpg.webp.lossy.webp'
File:      [doc-root]/wp-content/uploads/2015/08/image1xxl-32.jpg
Dimension: 870 x 1110
Output:    104128 bytes Y-U-V-All-PSNR 39.77 55.68 57.12   41.48 dB
           (0.86 bpp)
block count:  intra4:       1813  (47.09%)
              intra16:      2037  (52.91%)
              skipped:      1310  (34.03%)
bytes used:  header:            286  (0.3%)
             mode-partition:   9235  (8.9%)
 Residuals bytes  |segment 1|segment 2|segment 3|segment 4|  total
  intra4-coeffs:  |   84385 |      69 |      39 |      64 |   84557  (81.2%)
 intra16-coeffs:  |    8479 |     272 |      72 |     587 |    9410  (9.0%)
  chroma coeffs:  |     580 |       5 |       8 |      19 |     612  (0.6%)
    macroblocks:  |      56%|       1%|       1%|      42%|    3850
      quantizer:  |      26 |      20 |      15 |      11 |
   filter level:  |       8 |       5 |       2 |       0 |
------------------+---------+---------+---------+---------+-----------------
 segments total:  |   93444 |     346 |     119 |     670 |   94579  (90.8%)

Success
Reduction: 34% (went from 155 kb to 102 kb)

Converting to lossless
Locating cwebp binaries
1 cwebp binaries found in common system locations
Checking if we have a supplied binary for OS: Darwin... We do.
We in fact have 1
A total of 2 cwebp binaries where found
Detecting versions of the cwebp binaries found (and verifying that they can be executed in the process)
Executing: /usr/local/bin/cwebp -version. Result: version: 1.0.3
Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12 -version
Exec failed (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12)
Trying executing the cwebs found until success. Starting with the ones with highest version number.
Creating command line options for version: 1.0.3
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 80 -alpha_q '85' -near_lossless 60 -m 6 -low_memory '[doc-root]/wp-content/uploads/2015/08/image1xxl-32.jpg' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image1xxl-32.jpg.webp.lossless.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image1xxl-32.jpg.webp.lossless.webp'
File:      [doc-root]/wp-content/uploads/2015/08/image1xxl-32.jpg
Dimension: 870 x 1110
Output:    375904 bytes (3.11 bpp)
Lossless-ARGB compressed size: 375904 bytes
  * Header size: 4314 bytes, image data size: 371564
  * Lossless features used: PREDICTION CROSS-COLOR-TRANSFORM SUBTRACT-GREEN
  * Precision Bits: histogram=5 transform=4 cache=10

Success
Reduction: -137% (went from 155 kb to 367 kb)

Picking lossy
cwebp succeeded :)

Converted image in 1554 ms, reducing file size with 34% (went from 155 kb to 102 kb)
