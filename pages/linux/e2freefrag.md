# e2freefrag

> Print the free space fragmentation information for ext2/ext3/ext4 filesystems.
> More information: <https://manned.org/e2freefrag>.

- Check how many free blocks are present as contiguous and aligned free space:

`e2freefrag {{/dev/sdXN}}`

- Specify [c]hunk size in kilobytes to print how many free chunks are available:

`e2freefrag -c {{chunk_size_in_kb}} {{/dev/sdXN}}`
