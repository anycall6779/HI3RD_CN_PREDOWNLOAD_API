### 사전다운로드 API

```text
https://hyp-api.mihoyo.com/hyp/hyp-connect/api/getGameBranches?launcher_id=jGHBHlcOq1
```

응답에서 `biz=bh3_cn` 선택:

```text
game_id:    osvnlOc0S8
package_id: jdEaAE9pKa
branch:     predownload
password:   OAvMeb9icV0x
tag:        9.1.0
```

실제 Sophon 사전다운로드 API:

```text
https://api-takumi.mihoyo.com/downloader/sophon_chunk/api/getBuild?branch=predownload&package_id=jdEaAE9pKa&password=OAvMeb9icV0x
```

Sophon API의 `branch=predownload` 방식은 공개 분석 문서에도 확인됩니다. ([API 형식 참고](https://blog.amarea.cn/archives/genshin-launcher-chunk-download-mode.html/comment-page-1?replyTo=333))
