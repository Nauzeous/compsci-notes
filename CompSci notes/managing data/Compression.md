
Compression helps with 4 things:
- reducing file size
- reducing download times
- reducing storage requirement
- making best use of bandwidth

The bandwidth of your internet will often be a bottleneck when trying to upload or download files, which means that optimising files for limited bandwidth is important, and makes it much faster to transmit across the internet

There are 2 types of compression:
- ==Lossy==
- ==Lossless==

Lossy means that actual data is lost when compressing, and the compressed result cannot be uncompressed to recreate the original file
Lossless means that no data is lost, and is instead represented more efficiently

Lossy compression results in smaller files with lower quality
Lossless compression results in larger files with higher quality

Lossy compression is an acceptable compromise of quality against file size for audio, images, and videos, as reductions in quality are less noticeable

Lossless compression doesn't sacrifice any quality during compression, and does this by shortening repeated pieces of information

## Example

![](https://lh7-us.googleusercontent.com/Rf-ZYzw3SHLLry0LKfUWAGQgZtqrfr0z78vgp9VaIYZqIVsQBwpoX_jgMtMojI1qvvrNk8UJy3I5FGo0FaW53H4soYBgdMFeBlw3O2QuMyDZ5pYTZ0SftjnUWdMD2eQWkgVaCH8hoQ68UZDyQmoTlCBEAQ=s2048)

This first row can be represented as a string of 2 white pixels, 3 blue pixels, 7 white pixels, 3 blue pixels, and 2 white pixels, instead of individually storing each pixel

if the code for white is 111 and the code for blue is 001, you can represent the first line as 111==10== 001==11== 111==111== 001==11== 111==10==
where the highlighted part represents how many times the colour code is repeated 

By doing this, you can reduce the number of bits used, resulting in smaller files with identical quality

However this method only works on images with long chains of continuous colours
This means that lossless compression is ideal for computer graphics like cartoons, logos and icons, but are less effective at compressing full colour real photographs as there are very few blocks of repeating colours

## File types and compression

The file type often determines which method of compression is ideal, as some files are not suited for lossy compression

An example is text documents, you cannot afford to lose any data via compression, meaning lossless compression must be used

## Comparison

Compression:
- reduces file size
- makes files quicker to transfer
- reduces space taken up in storage

Lossy compression:
- data is lost in compression
- loss in quality
- **significantly reduces file size**
- suitable for images, audio, videos

Lossless compression:
- No data is lost
- The original file can be recreated 
- **inconsistent reduction in file size**
- suitable for .exe files and text documents


Two methods of lossless compression:
- Dictionary encoding
- Run-length encoding

dictionary encoding is better at compressing text based documents 
Run-length encoding is better at compressing images

### Dictionary encoding

dictionary encoding works by creating an index for each data item

For a text document, a word can be represented by a unique code

the message "One fish two fish red fish blue fish" can be turned into a table of words, removing duplicates

	1 One
	2 fish
	3 two
	4 red
	5 blue

and the message becomes '1 2 3 2 4 2 5 2' and can be used to recreate the original file

### Run-length encoding

run length encoding works by representing contiguous pixels of the same colour using a single pixel and stating how many times it is repeated, like a for loop.
by being able to represent multiple same colour adjacent pixels, you can save space by only using one value for a pixel and telling it how many times it needs to be used, as opposed to storing each pixel individually

run-length encoding is inconsistent at reducing file size, and works best for vector graphics or computer graphics with many contiguous same-colour pixels, as realistic images often have many gradients and a large colour depth