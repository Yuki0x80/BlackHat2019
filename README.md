#BlackHat2019
memo

# first Sesstion
Privilege escalation bugs
  Restricted user Call -> System Service(RPC) -> Tergetfile

CVE-2018-8440 [GitHub - sourceincite/CVE-2018-8440: CVE-2018-8440 standalone exploit](https://github.com/sourceincite/CVE-2018-8440)
DACL rewrite
call SchRpcSetSecurity win.iniから

TOCTOU Read file(CVE-2019-0636)
ReadDirectoryChangesW
no login
ブルーとフォースする

Trigger function call?
> windows
>
UI actions SetSecurity Call detected
Replace the path
start call function

Replace settgins file hardlin + App = Attack
DSLから

Bug＃３
windows defendersSercie　→ button → Current threats → set DACL for virus file

PainText ABC → DSLを特別な権限にする。

＠tｍｂｋｅｅｐｅｒ. Xuanwu Lab Tencent



Specker [Tencent Security Xuanwu Lab](https://xlab.tencent.com/en/)



権限昇格バグのお話

 [GitHub - sourceincite/CVE-2018-8440: CVE-2018-8440 standalone exploit](https://github.com/sourceincite/CVE-2018-8440)
Windowsの権限昇格の話でMicrosoft Windows タスクスケジューラの SchRpcSetSecurity API には、Advanced Local Procedure Call (ALPC) の処理に脆弱性が存在します。認証されたユーザによって、ACL (Access Control List、アクセス制御リスト) で保護されているファイルを上書きされ、SYSTEM 権限を取得される可能性があります。

[](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2019-0636)
TOCTOU（Time-of-check　to time-of-use）
競合状態を利用したバグである。
一人がアクセスし、そのあと他の人がアクセスした後に最初の人がファイルをロックした場合は、後の人は編集を行っても内容は反映されます。これを利用して、ファイル内のファイル内容を読み取るという脆弱性


これを利用することで
DACLでマルウェアのファイルの権限を昇格させる。


########################
Simからoperater,operaterから他のオペレータにアクセスする
Back Account Hackers Userd SS7 to intercept Security Code

SS7ファイアーフォール。
SS7ファイアーフォールからHLRに互いに通信を行い、OpenSSHを利用している。

SS7ファイアーフォールにSIGTRAN ＜ーリバースエンジニアリング、ファジング、exploit

SS7のプロトコル、Map,TCAP、SCCP、MTP3,２、１、PHY

IP/SCTP FOR an ss7 firewall
SCCP レガシーなプロトコル
NTPルーチンを利用したもの、Gobal title iphoneや携帯特有番号が含まれる

Sccp Tasks For SS7
SccpMessage,0,2,3,5 unsigred shortバイトしか受け付けない。

digits (size bytes) => オーバーフローさせて、attack Codeを呼び込む

TCAP/MAP
opecodeをオーバフローすることができる。
リモートエクスプロイトすることができる。


#Project Zero
セキュリティ研究チームである。Make ０day　Hard

良い防御はdetailed knowledge of offens.
良い防御は、詳細な攻撃を知っている。

防御より、attackerの方がbenefit

最新の産業は、規範を率いて、改善しているセキュリティ

チームオペレーション。
自分で何を仕事したいのかを決める。

Manual 54.2 Fuzzing 37.2 Other 8.6

新しい脆弱性を見つけるには、
Find bugs faster than we currently are,or
Find bugs that we cant currently surface

exploitのテクニックを学習する。共有する。

ドキュメント出会ったり、良いサンドボックス環境や、プロセスの改善

Classic Hits

Cause/effect

Spectre and meltdown by hann horn

task_t considered harmful
XNU kernel privilege escalation

200+ Flash UaF,OOB R/W

MPEngine and WPAD now sandboxed

Broadcom WiFi
android 25 byte linear overflow
ios 16bit incremants up to 60bytes past alllocated buffer.

最先端の私的状態のために分岐する
project0は可視化する。
open attack resarch provides the best path forward for make 0day hard

決して脆弱性についての討論は終わらない、

どのように推奨するか、改善するモデルを

私は、知らせる見つけた方法を増加させる名誉と楽しさのレベル、仕事をすることに対して、その狙いは、その仕組みを保持することが大事である。


脆弱性を作ってしまう人と、バグを発見する人の戦いは、有効なゴールはある。

否定的な結果を受け入れて祝う

脆弱性に関しては、問題を知らせ、研究者同士や一般に状況をシェアーしパッチのギャップを減らす。


hawkes



##### API-induced SSRF

SSRF Refresher
Get /foo -> sensitive data

GCP or AWS box -> GETs accessToken and explires code token Type

SMTP throught gopher:// URLs

Apple pay
in-store in-app Web

vlidationURL xx/foo 商人がサーバ（DNS？）を抑える。

Demos
Payment Request API wrapper for apple 論文

リクエストにdata-binary ふよ、
SSRF でリクエストヘッダを別のものに入れ替える。SRFF

リクエストををいただいて、validation-URLを書き換える。

check validation URL against applie list
Strip and Braintree handle

User regex domain
Regex like https?://.*.apple/

WebHooks
Request URL は下記になっている
http://169//
gopher://localhost:11211/....

HMAK and hope listerner checks it lots of Webhooks do this

Who filed to check the Hmack

Recieve and DOwnload MMS Messages

What did i do
repositoryURL=
message,
URLjavascirpt:alert("xss")

有効なMACと無効なMacをそれぞれ投げてテストする。

## Ghidra - Journey from Classified NSA Tool to Open Source


[GitHub - NationalSecurityAgency/ghidra: Ghidra is a software reverse engineering (SRE) framework](https://github.com/NationalSecurityAgency/ghidra)

BRAIN KINGHTON CHEIS DELIKAT

NSA Mission
サイバーセキュリティ犯罪を守る。 支援、

ギードラ ３首ドラゴン

IDAと同じ感じ、Windows　Tool
Function Graph や Comment などなどができる
どのプロセッサーでも動く

スクリプトマネージャもあるPython Java

windowsを複数の画面に分割することができる

Memory Symbol table ...

Docking windows
java GUI Gtree Gtable,

2003年から開発が始まって、9.x 2019

#######
Gole IDA and Hex-Rays allocated
自動的にapply informationを作成する。

Dynamic Structure Reconstructions

imp_free dword -> hook

metadata in tree(map) structure
forget removes items from the tree

頻繁にアクセスしているサイズ

PTE
Track eve allocation ala DBI
only ..

Simply add breckpoint upon memcopyなど

memoryが増加すれば、pegefalutが起きる。


全ての関数をフックして、自分の任意のDLLを呼び出す。





memo: /Users/saiyuki1919/jython2.2.1

# Government Malware

Goverment malware mallicious softwre

Lawful intercept Rats and 0day

ISPs to send phishing text messages to install spyware on target device

Google store でへんな Spywareを発見した

それは、malicious apps?
ユーザのハードウェアにマルウェアが発見されたというお話。
上記のことは起こりうる

２５mailicious apps on Google play sore
被害者は1000人

マルウェアは以下のことをした。
IMEI and Phone Number CheckValidTarget

すぐにアップデートをおこなっった
Malwareをダウンロードして、ペイロードを実行した。

SMS,や写真や電話、などなどを取得していた。

同じネトワークの端末が感染した。

被害者の端末にデータはなかった。 どうやって端末にインストールされたのかがわからなかった

deviceハッキングはNSA FSBがやってんじゃないか？
どうしたら良い？

ジャーナリストに連絡した。

facivonをshodan ４０サーバからモドあった・
e-SURV
agent appication gather data forom android send C&C

eSurv Secretly develops malware called exodus

eSurv spyware called Exodus

イタリアはマルウェアマーケットになっている。

inquiry　して、違法な盗聴として　行ったが無罪
おフィルは存在しなかった。

検察官のみアクセスすることができた。

use Government Trojans

政府は、2000にはマルウェアを使っていた。

1999年にアメリカもマルウェアを使っていた、Carnivore
PGPを盗んでいた。
2007年はCIPAVを使っていた。

マーケットでは、中国が攻撃的に向かっているなっている。

暗号化は古い盗聴を時代遅れにします
swborders
lorenzofb



## Exploit the Nwe WOrkd Remote Exploitation SQLite

Fuzzing for SQLite
FTS3/4/5 RTREE use shadow tabels store content

Nodes(BLOBs) Definitions
Dolist Format

CVE-2018-20346
memcpy in LN310 seems vulnerable

CVE-2018-20506
fts3ScanInterriorNodeに脆弱性
これもヒープオーバーフロー
64bits heap spray

CVE-2018-20505
fts3SegReaderNext
nPrefix + nSuffix integer overflows

libcurl
Protocols fulfill our requirements
FTP,HTTPSNTLM over HTTP

CVE-2018-1689
CVE-2019-3822
ntlmbuf is a stack variant
integer overflow
stack overflow

CVE-2019-3822
ntresp_len is set by len
Curl_auth_create_ntlm_type3_message

buffer overflow



