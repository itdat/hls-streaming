mkdir [hash_code]
ffmpeg -i [input_file.mkv] -profile:v baseline -level 3.0 -start_number 0 -hls_time 10 -hls_list_size 0 -f hls [hash_code]\index.m3u8
ffmpeg -i [input_file.mkv] -ss 00:00:01 -vframes 1 [hash_code].jpg
