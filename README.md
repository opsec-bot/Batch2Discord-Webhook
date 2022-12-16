# Batch2Discord-Webhook

edit your embed in message.json
this is meant to be used in other batch programs 

```@echo off   
set WEBHOOK=https://discord.com/api/webhooks/1053435886706110475/vb4uk6_P81Cxj2rTNaAA6E9QW6Q1PmZvE5DNT-nmtkTr-n2IaYQHAWDROgJKrkqh79Y2

curl -X POST -H "Content-Type: application/json" -d @message.json %WEBHOOK%


if %ERRORLEVEL% NEQ 0 (
    echo Curl command failed with error code %ERRORLEVEL%.
    exit /b %ERRORLEVEL%
)
```
where it says `WEBHOOK=` after the equal sign (=) paste your webhook their after removing mine.
