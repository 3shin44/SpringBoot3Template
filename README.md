# Spring Boot 3 Template Structure

## 專案說明
基於 Spring Boot 3，整合以下常用功能

- 查詢版本號 HTTP 接口: 提供簡單的 HTTP API，用於查詢應用程式的當前版本號。
- 非預期 HTTP Request 處理: 針對未定義的 HTTP 請求進行統一處理。
- 輸出 LOG 至檔案: 支援日誌輸出至檔案，依據日期產生並限制大小。
- 自動排版 (使用spotless & googleJavaFormat): 執行指令`mvn spotless:apply`

## 環境與結構

### 環境
- JAVA 17+
- Maven 3.8+

### 目錄結構
```
├─src
└──main
  ├─java
  │  └─com
  │      └─practice
  │          ├─controller 
  │          ├─service
  │          └─util // 共用函式, 如: Logger工具
  └─resources
     ├─static
     └─templates
```