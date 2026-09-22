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

### TEXTMAP 확인 결과

Manifest에는 `TextMap` 파일명이 직접 노출되지 않습니다.

하지만 `10161 / matching_field=game` Manifest 내부에 다음 ASB가 포함됩니다.

```text
BH3_Data/StreamingAssets/Asb/pc/954ca744edf85ea0.wmv
size: 40077391
md5:  a6fcd86397a0afabd08eaab5847f205c
```

AssetStudio로 추출한 결과:

```text
assetstudio_predl_textassets_20260922/
└─ 954ca744edf85ea0/
   └─ TextAsset/
      └─ TextMapGameStart.dat
```

검증값:

```text
size: 15016
md5:  dc2bb7bcc6303ab9b3ef644ffb950578
```

predownload_api_20260922\live_textmap_check.json
predownload_api_20260922\REPORT.md
```
