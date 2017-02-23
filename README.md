# test-hash

https://shattered.it/

Too bad git hashes aren't done with a straight SHA-1 or we'd see what might happen here.

http://stackoverflow.com/questions/460297/git-finding-the-sha1-of-an-individual-file-in-the-index#answer-24283352


It seems that the whole "blob content-size\0CONTENT" is a newer format. Old git stored it as the direct hash. If git implements a compatibility layer....?
