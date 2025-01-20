# TD2DecTech

## Questions Part I
Q1 - Create a torrent containing this image.

Q2 - Now copy the image to a new directory named partition1 and create a torrent of this folder. What do you observe?

The generated torrent file references the folder partition1, and its metadata reflects both the directory structure and the file content.


Q3 - Copy the partition1 folder and then generate the associated torrent. What do you observe?

The generated torrent for partition1_copy will have identical file data and structure but a different hash because the torrent metadata includes the path and potentially timestamp information.


## Questions Part II
Be sure to have download IPFS Desktop and IPFS CLI before starting this section

Q1 - Upload the previous image to IPFS.

CID : QmeJaufp9seXCpHMFwxX53P3oRQW8Ny1DduCXAxebEwxv7

This CID uniquely represents the file's content and allows it to be retrieved from any IPFS node.

Q2 - Now upload partition1 to IPFS. What do you observe compared to the torrent part?

- Unlike a single file, the folder's CID includes metadata about its structure and all its contents.
- Like torrents, if the content or folder structure changes, the CID will change.
- However, IPFS does not require .torrent files or trackers; it uses the CID directly for content addressing and retrieval.
- 
Q3 - Copy the partition1 folder and then generate the associated torrent. What do you observe?
- If the folder's structure and content are identical, the CID for partition1_copy will be the same as the CID for partition1.
- IPFS uses Content Addressing, ensuring that identical data always results in the same CID.


