# PTTCrawler
試看看PTT的爬蟲，用爬蟲分析看看最近的爆文是否有異常的情況
==

需求模組:
--
PTTLibrary,json,numpy,pandas

執行方式:
-
調整完參數之後直接python執行

1_AbnormalBowWenAnalyzer_Ver1_X.py和settings.json需要在同一目錄底下

V1.1更新:
-
增加搜尋特定ID的功能

搜尋特定ID時最後結果會顯示這個ID爆文的篇數比率

以及這個ID的文章中第目標則推文與發文時間差距小於GapBoundary的篇數比率

V1.2更新:
-
多了ID統計的功能


參數設定: 
--
在**settings.json**中

ID:PTT帳號

Password:PTT密碼

pushBoundary:分析超過多少則推的文

Board:分析哪個版

StartIndex:要分析的起始文章編號

EndIndex:要分析的結束文章編號

showPushTime:是否要顯示推文的時間(只會顯示GapPrint/25/50/75這幾則推文的時間)

GapPrint:第GapPrint則數的推文小於GapBoundary才會顯示,0則只要超過pushBoundary則推文即會顯示

GapBoundary:第GapPrint則推文與發文時間的差距，單位為分鐘，小於此時間的才會顯示出來

SearchID:是否要搜尋特定ID(Bool值)

TargetID:要搜尋的目標ID(String),在SearchID為True時才會有用

CalUnderPush:指定數量以下的推文ID會被統計(int)
