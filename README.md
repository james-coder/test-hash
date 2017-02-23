# test-hash

https://shattered.it/

Too bad git hashes aren't done with a straight SHA-1 or we'd see what might happen here.

http://stackoverflow.com/questions/460297/git-finding-the-sha1-of-an-individual-file-in-the-index#answer-24283352


It seems that the whole "blob content-size\0CONTENT" is a newer format. Old git stored it as the direct hash. If git implements a compatibility layer....?

If you ever got "lucky" enough, this would be your "prize"!
https://github.com/git/git/blob/1d1bdafd64266e5ee3bd46c6965228f32e4022ea/builtin/index-pack.c#L745

"SHA1 COLLISION FOUND WITH ____!"

https://github.com/git/git/blob/35f6318d44379452d8d33e880d8df0267b4a0cd0/pack-objects.c#L59

"BUG: Duplicate object in hash"


Also: 9239ad1980d44e79bf137fe50b71af74eca34f
