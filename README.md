# PTTCrawler
試看看PTT的爬蟲，用爬蟲分析看看最近的爆文是否有異常的情況
==

需求模組:
--
PTTLibrary,json,numpy,pandas

執行方式:
-
調整完參數之後直接python執行



參數設定: 
--
在settings.json中

ID:PTT帳號

Password:PTT密碼

pushBoundary:分析超過多少則推的文

Board:分析哪個版

StartIndex:要分析的起始文章編號

EndIndex:要分析的結束文章編號

showPushTime:是否要顯示推文的時間(只會顯示GapPrint/25/50/75這幾則推文的時間)

GapPrint:第GapPrint則數的推文小於GapBoundary才會顯示,0則只要超過pushBoundary則推文即會顯示

GapBoundary:第GapPrint則推文與發文時間的差距，單位為分鐘，小於此時間的才會顯示出來

