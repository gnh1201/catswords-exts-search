# catswords-exts-search
![exts.kr is the data format community since 2008](https://ics.catswords.net/catswords-exts-logo.png) catswords-exts-search REST API docs

## Background
These data have served as file format metadata since 2008, when I was a student aspiring to pursue a career in computer science, and throughout my professional career ever since.

Initially, they were hosted on a standalone website, but maintaining it with the latest technology stack became challenging. To ensure continued accessibility, I have now made them publicly available using Microsoft Azure's AI Search platform.

Even today, I believe they will remain valuable for various applications, including Retrieval-Augmented Generation (RAG) for file format preprocessing.

## Public API keys
Due to GitHub's security policy, public API keys cannot be disclosed here. Instead, they are available on [our Discord channel](https://discord.gg/8JUzMCmRzr).

## Try search (keyword: ransomware)

### Request

`POST https://catswords-exts-search.search.windows.net/indexes/azuresql-index/docs/search?api-version=2016-09-01`

```bash
curl 'https://catswords-exts-search.search.windows.net/indexes/azuresql-index/docs/search?api-version=2016-09-01' \
  -H 'api-key: YOUR_API_KEY' \
  -H 'content-type: application/json' \
  --data-raw '{"search": "ransomware","count": true,"top": 3}'
```

### Response

```json
{
  "@odata.context": "https://catswords-exts-search.search.windows.net/indexes('azuresql-index')/$metadata#docs(*)",
  "@odata.count": 8314,
  "value": [
    {
      "@search.score": 24.083279,
      "id": "10278",
      "prefix": "M",
      "identifier": "MOSK",
      "content": "STOP (DJVU) ransomware encrypted file",
      "flag": "NULL",
      "description": "STOP (DJVU) ransomware encrypted file",
      "organization": "STOP/DJVU ransomware family",
      "mime": "NULL",
      "execution": "STOP (DJVU) ransomware",
      "signature": "ATTENTION!\n\nDon't worry, you can return all your files!\nAll your files like photos, databases, documents and other important are encrypted with strongest encryption and unique key.\nThe only method of recovering files is to purchase decrypt tool and unique key for you.\nThis software will decrypt all your encrypted files.\nWhat guarantees you have?\nYou can send one of your encrypted file from your PC and we decrypt it for free.\nBut we can decrypt only 1 file for free. File must not contain valuable information.\nYou can get and look video overview decrypt tool:\nhxxps://we.tl/t-7cpJN3gq4f\nPrice of private key and decrypt software is $980.\nDiscount 50% available if you contact us first 72 hours, that's price for you is $490.\nPlease note that you'll never restore your data without payment.\nCheck your e-mail \"Spam\" or \"Junk\" folder if you don't get answer more than 6 hours.\n\n\nTo get this software you need write on our e-mail:\nrestoredatahelp@firemail.cc\n\nReserve e-mail address to contact us:\ngorentos@bitmessage.ch\n\nYour personal ID:",
      "programid": "NULL",
      "openwith": "STOP (DJVU) ransomware",
      "link1": "https://asec.ahnlab.com/1262",
      "link1_scheme": null,
      "link2": "https://www.pcrisk.com/removal-guides/16281-mosk-ransomware",
      "link2_scheme": null,
      "hit": 802,
      "tags": "NULL",
      "writer_ip": "MASKED",
      "status": "published",
      "enabled_ioc": 0,
      "created_on": "2019-11-21T01:26:38Z",
      "updated_on": "2019-11-21T01:26:38Z"
    },
    {
      "@search.score": 23.820217,
      "id": "6085",
      "prefix": "R",
      "identifier": "RYK",
      "content": "Ryuk ransomware was first detected in August 2018 and is spread via highly targeted attacks, although the infection method is currently unknown. According to Check Point researchers, when Ryuk infects a system, it kills over 40 processes and stops more than 180 services by executing taskkill and net stop on a list of predefined service and process names. Additionally, Ryuk requires Admin privileges to run and maintains persistence by writing itself to the Run registry key. Researchers have noted several similarities to the Hermes ransomware, suggesting that the recent Ryuk campaigns may be related to the Hermes operators or another threat actor who has obtained the Hermes source code. Some of the similarities between Hermes and Ryuk include the same file marker for encrypted files, similar whitelisted folders, and a similar script to delete shadow volumes and backup files. Ransom demands have varied among victims, ranging from 15 BTC to 50 BTC, with a combined profit of over $640,000 in bitcoin generated from victim payments.",
      "flag": null,
      "description": "Ryuk ransomware",
      "organization": "Lazarus",
      "mime": null,
      "execution": "Ryuk ransomware",
      "signature": "RyukReadMe.txt, UNIQUE_ID_DO_NOT_REMOVE.txt\nMelisaPeterman@protonmail.com\nMelisaPeterman@tutanota.com\neliasmarco@tutanota.com\nCamdenScott@protonmail.com",
      "programid": null,
      "openwith": "Ryuk ransomware",
      "link1": "https://www.cyber.nj.gov/threat-profiles/ransomware-variants/ryuk",
      "link1_scheme": null,
      "link2": "https://www.boannews.com/media/view.asp?idx=75927&amp;utm_source=dable",
      "link2_scheme": null,
      "hit": 761,
      "tags": "NULL",
      "writer_ip": "MASKED",
      "status": "published",
      "enabled_ioc": 0,
      "created_on": "2019-01-16T01:58:29Z",
      "updated_on": "2019-01-16T01:58:29Z"
    },
    {
      "@search.score": 23.521881,
      "id": "10192",
      "prefix": "E",
      "identifier": "ENC_ROBINHOOD",
      "content": "Officials in Baltimore said Tuesday the city was the victim of a ransomware attack that has knocked out several services, including municipal employees’ emails, phone lines and online bill payments. Mayor Bernard C. “Jack” Young said the city has also shut down the majority of its computer servers “out of an abundance of caution.”\nThe incident marks the second time in as many years that Baltimore has fallen prey to a cyberattack. The city’s 911 and 311 systems were hacked in March 2018, forcing dispatchers to take manual notes on emergency calls for several days.",
      "flag": "NULL",
      "description": "RobinHood ransomware encrypted file",
      "organization": "RobinHood",
      "mime": "NULL",
      "execution": "RobinHood ransomware encrypted file",
      "signature": "3bc78141ff3f742c5e942993adfbef39c2127f9682a303b5e786ed7f9a8d184b\n\nAVP, MMS, ARSM, SNAC, ekrn, KAVFS, RESvc, SamSs, W3Svc, WRSVC, bedbg, masvc, SDRSVC, TmCCSF, mfemms, mfevtp, sacsvr, DCAgent, ESHASRV, KAVFSGT, MySQL80, POP3Svc, SMTPSvc, Smcinst, SstpSvc, TrueKey, mfefire, EhttpSrv, IISAdmin, IMAP4Svc, McShield, MySQL57, kavfsslp, klnagent, macmnsvc, ntrtscan, tmlisten, wbengine, Antivirus, MSSQL$TPS, SQLWriter, ShMonitor, UI0Detect, sophossps, MSOLAP$TPS, MSSQL$PROD, SAVService, SQLBrowser, SmcService, swi_filter, swi_update, AcrSch2Svc, EsgShKernel, MBAMService, MSSQLSERVER, MsDtsServer, SntpService, VeeamNFSSvc, swi_service, AcronisAgent, FA_Scheduler, MSExchangeES, MSExchangeIS, MSExchangeSA, MSSQL$ECWDB2, MSSQL$SOPHOS, MSSQL$TPSAMA, PDVFSService, ReportServer, SQLAgent$TPS, SQLTELEMETRY, VeeamRESTSvc, MSExchangeMTA, MSExchangeSRS, MSOLAP$TPSAMA, McTaskManager, SQLAgent$CXDB, SQLAgent$PROD, VeeamCloudSvc, VeeamMountSvc, SQL Backups, mozyprobackup, msftesql$PROD, swi_update_64, EraserSvc11710, MSExchangeMGMT, MSSQL$BKUPEXEC, MSSQL$SQL_2008, MsDtsServer100, MsDtsServer110, SQLSERVERAGENT, VeeamBackupSvc, VeeamBrokerSvc, VeeamDeploySvc, Sophos Agent, svcGenericHost, EPUpdateService, MBEndpointAgent, MSOLAP$SQL_2008, MSSQLFDLauncher, McAfeeFramework, SAVAdminService, SQLAgent$ECWDB2, SQLAgent$SOPHOS, SQLAgent$TPSAMA, VeeamCatalogSvc, MSSQL$SHAREPOINT, MSSQL$SQLEXPRESS, MSSQL$SYSTEM_BGC, NetMsmqActivator, ReportServer$TPS, SepMasterService, TrueKeyScheduler, EPSecurityService, MSOLAP$SYSTEM_BGC, MSSQL$PRACTICEMGT, SQLAgent$BKUPEXEC, SQLAgent$SQL_2008, SQLSafeOLRService, VeeamTransportSvc, Zoolz 2 Service, MSSQL$PRACTTICEBGC, MSSQL$VEEAMSQL2012, Sophos MCS Agent, BackupExecJobEngine, MSSQL$SBSMONITORING, MSSQLFDLauncher$TPS, MSSQLServerADHelper, McAfeeEngineService, OracleClientCache80, ReportServer$TPSAMA, SQLAgent$SHAREPOINT, SQLAgent$SQLEXPRESS, SQLAgent$SYSTEM_BGC, SQLTELEMETRY$ECWDB2, Sophos MCS Client, BackupExecRPCService, MSSQL$VEEAMSQL2008R2, TrueKeyServiceHelper, BackupExecVSSProvider, MSSQL$PROFXENGAGEMENT, ReportServer$SQL_2008, SQLAgent$PRACTTICEBGC, SQLAgent$PRACTTICEMGT, SQLAgent$VEEAMSQL2012, BackupExecAgentBrowser, MSSQLFDLauncher$TPSAMA, MSSQLServerADHelper100, MSSQLServerOLAPService, SQLAgent$SBSMONITORING, VeeamDeploymentService, VeeamHvIntegrationSvc, Acronis VSS Provider, Sophos Clean Service, ReportServer$SYSTEM_BGC, SQLAgent$VEEAMSQL2008R2, Sophos Health Service, Sophos Message Router, MSSQLFDLauncher$SQL_2008, SQLAgent$PROFXENGAGEMENT, SQLsafe Backup Service, SQLsafe Filter Service, SQLAgent$CITRIX_METAFRAME, VeeamEnterpriseManagerSvc, BackupExecAgentAccelerator, MSSQLFDLauncher$SHAREPOINT, MSSQLFDLauncher$SYSTEM_BGC, Sophos Safestore Service, Symantec System Recovery, BackupExecManagementService, Enterprise Client Service, Sophos AutoUpdate Service, BackupExecDeviceMediaService, Sophos Web Control Service, MSSQLFDLauncher$SBSMONITORING, Sophos File Scanner Service, McAfeeFrameworkMcAfeeFramework, MSSQLFDLauncher$PROFXENGAGEMENT, Sophos Device Control Service, Sophos System Protection Service, Veeam Backup Catalog Data Service, \n\nWhat happened to your files?\nAll your files are encrypted with RSA-4096, Read more on https://en.wikipedia.org/wiki/RSA_(cryptosystem)\nRSA is an algorithm used by modern computers to encrypt and decrypt the data. RSA is an asymmetric cryptographic algorithm. Asymmetric means that there are two different keys. This is also called public key cryptography, because one of the keys can be given to anyone:\n\n1 - We encrypted your files with our \"Public key\" \n2 - You can decrypt, the encrypted files with specific \"Private key\" and your private key is in our hands ( It's not possible to recover your files without our private key )\n\nIs it possible to get back your data?\nYes, We have a decrypter with all your private keys. We have two options to get all your data back.\nFollow the instructions to get all your data back:\n\nOPTION 1\nStep 1 : You must send us 3 Bitcoin(s) for each affected system\nStep 2 : Inform us in panel with hostname(s) of the system you want, wait for confirmation and get your decrypter\nOPTION 2\nStep 1 : You must send us 13 Bitcoin(s) for all affected system\nStep 2 : Inform us in panel, wait for confirmation and get all your decrypters\n\nOur Bitcoin address is: xxx \n\nBE CAREFUL, THE COST OF YOUR PAYMENT INCREASES $10,000 EACH DAY AFTER THE FOURTH DAY\n\nAccess to the panel ( Contact us )\nThe panel address: http://xbt4titax4pzza6w.onion/xx/\n\nAlternative addresses\nhttps://xbt4titax4pzza6w.onion.pet/xx/\nhttps://xbt4titax4pzza6w.onion.to/xx/\nAccess to the panel using Tor Browser\nIf non of our links are accessible you can try tor browser to get in touch with us:\nStep 1: Download Tor Browser from here: https://www.torproject.org/download/download.html.en\nStep 2: Run Tor Browser and wait to connect\nStep 3: Visit our website at: panel address\n\nIf you're having a problem with using Tor Browser, Ask Google: how to use tor browser\nWants to make sure we have your decrypter?\nTo make sure we have your decrypter you can upload at most 3 files (maximum size allowance is 10 MB in total) and get your data back as a demo.\nWhere to buy Bitcoin?\nThe easiest way is LocalBitcoins, but you can find more websites to buy bitcoin using Google Search: buy bitcoin online",
      "programid": "NULL",
      "openwith": "RobinHood ransomware",
      "link1": "https://www.bleepingcomputer.com/news/security/a-closer-look-at-the-robbinhood-ransomware/",
      "link1_scheme": null,
      "link2": "https://statescoop.com/robinhood-ransomware-knocks-out-city-services-in-baltimore/",
      "link2_scheme": null,
      "hit": 927,
      "tags": "NULL",
      "writer_ip": "MASKED",
      "status": "published",
      "enabled_ioc": 0,
      "created_on": "2019-05-26T08:55:00Z",
      "updated_on": "2019-05-26T08:55:00Z"
    }
  ]
}
```

## Try search (keyword: 영상)

### Request

`POST https://catswords-exts-search.search.windows.net/indexes/azuresql-index/docs/search?api-version=2016-09-01`

```bash
curl 'https://catswords-exts-search.search.windows.net/indexes/azuresql-index/docs/search?api-version=2016-09-01' \
  -H 'api-key: YOUR_API_KEY' \
  -H 'content-type: application/json' \
  --data-raw '{"search": "영상","count": true,"top": 3}'
```

### Response

```json
{
  "@odata.context": "https://catswords-exts-search.search.windows.net/indexes('azuresql-index')/$metadata#docs(*)",
  "@odata.count": 3,
  "value": [
    {
      "@search.score": 12.593983,
      "id": "10363",
      "prefix": "A",
      "identifier": "AMV",
      "content": "소형 MP3 및 MP4 플레이어에서 사용하는 Motion JPEG 기반의 동영상 파일이다.\n\n중국에서 만들어진 MP3 및 MP4 플레이어에 사용되고 있지만, 포맷이 처음에는 공개된 것이 아니어서 관련된 정보가 잘 알려지지 않았다.\n\n로열티에서 자유롭고 MP3 수준의 기기에서도 원활한 플레이가 가능하도록 설계되어 있다고 한다. 현재는 포맷 분석 과정을 통해 AMV를 처리할 수 있는 많은 방법이 나와있다.\n\n2020년 10월 기준, AMV 포맷을 이용하는 현재 판매되는 기기로는 <a href=\"https://coupa.ng/bLuQx5\">사파 SB1000</a>, <a href=\"https://coupa.ng/bLu8vF\">TJC BIT-550M</a>, <a href=\"https://coupa.ng/bLu8Hx\">MPGIO ATHENA Holic</a>, <a href=\"https://coupa.ng/bLu82J\">쉬크 U10</a>, <a href=\"https://coupa.ng/bLu9aq\">브리츠 BZ-MP4580BL</a>, <a href=\"https://coupa.ng/bLvazf\">비아이티셀택 BIT-401B</a> 등이 있다.\n\n<a href=\"https://coupa.ng/bLuQx5\">사파 SB1000</a> 모델의 경우 AMV로 변환된 2시간 분량의 인터스텔라(2014) 영화를 테스트했을 때 플레이하는데 전혀 문제가 없었다.\n\n인코딩 옵션은 보통 320x240/30fps, 160x120/16fps를 사용하는데, 앞서 언급한 기기에서는 160x120/16fps 옵션을 사용하면 된다. (30fps로 설정해도 플레이에는 문제가 없다.)\n\n자세한 인코딩 방법은 링크 #1를 확인하길 바란다.",
      "flag": "NULL",
      "description": "소형기기용 음악 및 영상 파일 (Anime Music Video File)",
      "organization": "Various",
      "mime": "NULL",
      "execution": "소형기기용 음악 및 영상 파일 (Anime Music Video File)",
      "signature": "NULL",
      "programid": "NULL",
      "openwith": "<a href=\"https://blog.naver.com/isc7981/222609967065\">FFmpeg</a>",
      "link1": "https://blog.naver.com/isc7981/222609967065",
      "link1_scheme": null,
      "link2": "https://wiki.multimedia.cx/index.php?title=AMV",
      "link2_scheme": null,
      "hit": 7240,
      "tags": "amv,mp3,mp4",
      "writer_ip": "MASKED",
      "status": "published",
      "enabled_ioc": 0,
      "created_on": "2020-10-23T11:22:54Z",
      "updated_on": "2022-01-01T18:52:52Z"
    },
    {
      "@search.score": 4.3085055,
      "id": "299",
      "prefix": "M",
      "identifier": "MP4",
      "content": "MPEG-4(엠펙 포, ISO/IEC 14496)는 영상, 음성을 디지털 데이터로 전송, 저장하기 위한 규격의 하나이다. MPEG-1, MPEG-2와 같이 시스템, 비주얼, 음향, 파일 포맷 규격으로 구성되어 있다. 그렇지만, 일반적으로 MPEG-4라고 할 때에는 동영상 인코딩 방식을 기술하는 비주얼 부분을 가리키는 경우가 많다.",
      "flag": null,
      "description": "MPEG-4 비디오 파일",
      "organization": null,
      "mime": null,
      "execution": "MPEG-4 비디오 파일",
      "signature": null,
      "programid": null,
      "openwith": null,
      "link1": null,
      "link1_scheme": null,
      "link2": null,
      "link2_scheme": null,
      "hit": 3601,
      "tags": "NULL",
      "writer_ip": "MASKED",
      "status": "published",
      "enabled_ioc": 0,
      "created_on": "2008-09-27T07:10:56Z",
      "updated_on": "2008-09-27T07:10:56Z"
    },
    {
      "@search.score": 1.4041742,
      "id": "762",
      "prefix": "D",
      "identifier": "DCM",
      "content": "의학분야에서 자기공명영상(MRI) 또는 컴퓨터 단층촬영(CT)의 결과를 표현한 파일이다.\n\n## DICOM 표준과 DCM 파일의 연관성\nDCM 파일은 DICOM 표준과 관련이 있으며, DICOM 표준의 오프라인 표현 파일이다. DICOM은 통신 표준을 정의하기 때문에 오프라인 표현 파일인 DCM 파일은 기존의 이미지 형식과 압축파일 포맷을 기반으로 하고있어 표준과 직접적인 연관이 있는 것은 아니다.\n\n현재 DICOM 오프라인 포맷(DCM)으로 저장되어지고 있는 자료 유형은 아래와 같다.\n\n- 디지털 방사선 촬영(CR, DX)\n- 유방촬영술(MG)\n- 컴퓨터 단층촬영(CT)\n- 자기 공명(MR)\n- 양전자 단층촬영 PET-CT(PT)\n- 초음파 검사(US)\n- 디지털 혈관조영(XA)\n- 감마선 카메라, 핵의학(NM)\n- 2차 생성 사진 및 스캔 이미지(SC)\n- Structured Reports (SR)\n\n기존의 이미지 형식과 압축파일 포맷을 따르고 있어 경우에 따라 아래 항목에 변동이 있을 수 있다.\n\n- 단색(CR, CT, MR) 및 컬러(US, 3D 재구성)\n- 정지 이미지(CR, MG, CT) 및 움직이는 이미지(XA, US)\n- 비압축 및 압축(RLE, JPEG Lossy, JPEG Lossless, JPEG 2000)\n\n## DCM 파일 복구와 관련된 정보\n확장자 정보를 남기면서 DCM 파일 복구에 대해 잠시 코멘트를 해보면, 기존의 이미지 형식과 압축파일 포맷을 따르고 있어 데이터 손실 시 바로 복구를 시도하면 복구율이 좋은 편이다.\n\n## DICOM 표준은 무엇일까?\n의료용 디지털 영상 및 통신(Digital Imaging and Communications in Medicine, DICOM) 표준은 의료용 기기에서 디지털 영상표현과 통신에 사용되는 여러 가지 표준을 총칭하는 말로, 미국방사선의학회(ACR)와 미국전기공업회(NEMA)에서 구성한 연합 위원회에서 발표한다.",
      "flag": null,
      "description": "MRI/CT(자기공명/컴퓨터단층) 촬영 파일",
      "organization": "미국전기공업회(NEMA), 미국방사선의학회(ACR)",
      "mime": null,
      "execution": "MRI/CT(자기공명/컴퓨터단층) 촬영 파일",
      "signature": null,
      "programid": null,
      "openwith": "RadiAnt",
      "link1": "https://www.radiantviewer.com/ko/",
      "link1_scheme": null,
      "link2": null,
      "link2_scheme": null,
      "hit": 5556,
      "tags": "dicom,dcm",
      "writer_ip": "MASKED",
      "status": "published",
      "enabled_ioc": 0,
      "created_on": "2017-10-24T04:09:45Z",
      "updated_on": "2017-10-24T04:09:45Z"
    }
  ]
}
```

## How to contribute
Contributions to this project are always welcome. Please visit the GitHub repository [gnh1201/catswords-exts-search](https://github.com/gnh1201/catswords-exts-search) and contribute. I appreciate reports on file formats, suggestions for applying new technologies, and any other contributions you may have.

## Contact me
- oss@catswords.net
- ActivityPub: [@catswords_oss@catswords.social](https://catswords.social/@catswords_oss)
- XMPP: [catswords@conference.omemo.id](xmpp:catswords@conference.omemo.id?join)
- Microsoft Teams: [Join Catswords OSS](https://teams.live.com/l/community/FEACHncAhq8ldnojAI)
- Discord: [#catswords-exts-search on Catswords OSS](https://discord.gg/8JUzMCmRzr)
