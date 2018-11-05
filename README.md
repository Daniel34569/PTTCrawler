# PTTCrawler
測試看看PTT的爬蟲

試著用爬蟲分析看看最近的爆文是否有異常的情況

參數設定: 

在settings.json中

ID:PTT帳號

Password:PTT密碼

pushBoundary:分析超過多少則推的文

Board:分析哪個版

StartIndex:要分析的起始文章編號

EndIndex:要分析的結束文章編號

showPushTime:是否要顯示推文的時間(只會顯示目標/25/50/75這幾則推文的時間)

GapPrint:

GapBoundary:第"目標"則推文與發文時間的差距，單位為分鐘，小於此時間的才會顯示出來

