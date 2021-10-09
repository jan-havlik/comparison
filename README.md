# comparison
Repository contaning data for the comparison of 2 R-loop algorithms

#### QmRLFS finder (**method**: `time` util)
- 100 kB `python2 QmRLFS-finder.py --model m1,m2 -i 100k.fasta -o 100k.out  20,49s user 0,02s system 99% cpu 20,512 total`
- 300 kB `python2 QmRLFS-finder.py --model m1,m2 -i 300k.fasta -o 300k.out  31,53s user 0,01s system 99% cpu 31,538 total`
- 500 kB `python2 QmRLFS-finder.py --model m1,m2 -i 500k.fasta -o 500k.out  50,03s user 0,02s system 99% cpu 50,065 total`
- 750 kB `109,8 s`
- 1 MB `python2 QmRLFS-finder.py --model m1,m2 -i 1m.fasta -o 1m.out  190,96s user 0,03s system 99% cpu 3:11,02 total`
- 3 MB `930 s`
- 5 MB `python2 QmRLFS-finder.py --model m1,m2 -i 5m.fasta -o 5m.out  1570,24s user 0,10s system 99% cpu 26:10,82 total`
- 10 MB `python2 QmRLFS-finder.py --model m1,m2 -i 10m.fasta -o 10m.out  2909,51s user 0,09s system 99% cpu 48:29,78 total`

#### DNA-Analyser (public server) (**method**: log diff)
- 100 kB
    - `2021-09-22 21:40:08 [http-nio-80-exec-1] /api/analyse/rloopr POST`
    - `2021-09-22 21:40:15 [http-nio-80-exec-3] /api/analyse/rloopr/df9d3cff-487b-4efc-9864-dc28190e6da4/heatmap?segments=80&from=0&to=100909 GET`
- 300 kB
    - `2021-09-22 21:44:56 [http-nio-80-exec-2]  /api/analyse/rloopr POST`
    - `2021-09-22 21:45:03 [http-nio-80-exec-2] /api/analyse/rloopr/e04d905f-dcf2-4eb9-9dd2-b3e1a23e496c/heatmap?segments=80&from=0&to=302824 GET`
- 500 kB
    - `2021-09-22 21:47:38 [http-nio-80-exec-8] /api/analyse/rloopr POST`
    - `2021-09-22 21:47:45 [http-nio-80-exec-8] /api/analyse/rloopr/ec49eb5d-f7a3-4f67-be12-682b49c77a63/heatmap?segments=80&from=0&to=504740 GET`
- 750 kB
    - `2021-09-23 21:11:13 [http-nio-80-exec-1] /api/analyse/rloopr POST`
    - `2021-09-23 21:11:24 [http-nio-80-exec-7] /api/analyse/rloopr/f2bfdfc0-ff72-4a5b-bbd7-25b8295d28c1/heatmap?segments=80&from=0&to=757134 GET`
- 1 MB
    - `2021-09-22 21:48:37 [http-nio-80-exec-3] /api/analyse/rloopr POST`
    - `2021-09-22 21:48:56 [http-nio-80-exec-5] /api/analyse/rloopr/18bdd6be-4a0a-40da-a046-128bfb731f2b/heatmap?segments=80&from=0&to=1033759 GET`
- 3 MB
    - `2021-09-23 21:08:29 [http-nio-80-exec-8] /api/analyse/rloopr POST`
    - `2021-09-23 21:09:28 [http-nio-80-exec-4] /api/analyse/rloopr/487e9ea9-502e-4615-a4ff-ecaf78a29a8f/heatmap?segments=80&from=0&to=3101373 GET`
- 5 MB
    - `2021-09-22 21:50:04 [http-nio-80-exec-1] /api/analyse/rloopr`
    - `2021-09-22 21:51:33 [http-nio-80-exec-5] /api/analyse/rloopr/fad9f599-c2d0-4ce3-95b7-a8a4d9968a81/heatmap?segments=80&from=0&to=5168988 GET`
- 10 MB
    - `2021-09-22 21:52:42 [http-nio-80-exec-3] /api/analyse/rloopr POST`
    - `2021-09-22 21:55:41 [http-nio-80-exec-9] /api/analyse/rloopr/84993753-a583-4133-aef6-4b3cb00bbea0/heatmap?segments=80&from=0&to=10338024 GET`
