# CEJC-DEP

## Description

発話単位の長単位・文節係り受けアノテーション

## Features

基本的には CaboCha 形式に長単位形態論情報・文節境界情報を追加したものです。

- #! DOC 行 ＜サンプル番号＞
- #! DOCID 行 ＜サンプル番号＞ ＜サンプル名＞ 
- #! DOCATTR 行
  - ＜DocInfo＞＜DialogID＞ サンプル名
  - ＜FileInfo＞＜File＞＜Speaker＞ 話者名
  - ＜FileInfo＞＜File＞＜FilePath＞ merge前ファイル名

- 係り受け情報行
  - 文節ID
  - 係り先文節ID
  - 係り受け関係ラベル
  - 自立語主辞オフセット
  - 付属語主辞オフセット

- EOS 行
  - EOS のみからなる文末情報

- 形態素行（タブ区切り）

  - 1列目：出現形

  - 2列目：短単位形態論情報（コンマ区切り）= MeCab-UniDic の出力と同等（但し、未定義のものは含まれません）

    - (0):  pos1
    - (1):  pos2
    - (2):  pos3
    - (3):  pos4
    - (4):  cType
    - (5):  cForm
    - (6):  lForm
    - (7):  lemma
    - (8):  orth
    - (9):  pron
    - (10): orthBase
    - (11): pronBase
    - (12): goshu
    - (13): iType
    - (14): iForm
    - (15): fType
    - (16): fForm
    - (17): iConType
    - (18): fConType
    - (19): type
    - (20): kana
    - (21): kanaBase
    - (22): form
    - (23): formBase
    - (24): aType
    - (25): aConType
    - (26): aModType
    - (27): lid
    - (28): lemma_id

  - 3列目：文節境界情報

## Authors

- 浅原正幸 (国立国語研究所)
- 若狭絢 (国立国語研究所)
- 大村舞 (国立国語研究所)

## Download

「中納言」サイト：日本語日常会話コーパスの備考に記載されている
「有償版契約者は関連データを[「データ配布」](https://cejc-data.ninjal.ac.jp/my/)からダウンロードできます。」から
ダウンロードしてください。

## Reference

浅原 正幸・若狭 絢, (2022), [『日本語日常会話コーパス』に対する係り受け情報アノテーション](https://www.anlp.jp/proceedings/annual_meeting/2022/pdf_dir/PT4-2.pdf), 言語処理学会第28回年次大会, p.1699-1703.

## License

CEJC の有償版契約に準じます

## Acknowledgement

本研究は国立国語研究所コーパス開発センター共同研究プロジェクトの成果です。
また、科研費17H00917・18H05521の支援を受けました。