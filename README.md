### https://study.hunet.co.kr/Study/Mov/JWplayer.aspx?chapterNo=0101&indexNo=5&current_frame_count=1&mov_Path=&progressNo=5&onlyMovSeamlessYn=Y&onlyMovYn=Y&duplicate_study_top_guid=#
- `0101` ~
- developer tool (shiif + cmd + i)
- brake point if
```
if (event.offset > maxPlayPosition) {
    seeking = true;
    setTimeout(function () {
        jwplayer('video').seek(maxPlayPosition);
    }, 5);
    isPause = false;
}
```
- player: seek 하기
- console 에 입력
```
maxPlayPosition = Math.round(jwplayer('video').getDuration()) - 10;
```
