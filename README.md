# 🛡️ Security Patterns for AI Security Scanner

> **오픈소스 보안 패턴 데이터베이스**  
> AI 보안 스캐너용 정적/동적 분석 패턴 모음

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Patterns](https://img.shields.io/badge/Patterns-61-blue.svg)]()
[![Languages](https://img.shields.io/badge/Languages-3-green.svg)]()

---

## 📋 개요

이 저장소는 **AI Security Scanner**에서 사용하는 보안 패턴과 페이로드를 제공합니다.

- **프로그램**: [웹사이트에서 다운로드](https://yourwebsite.com/pentest-agent)
- **패턴**: 이 저장소 (무료 오픈소스)

---

## 📦 포함된 파일

### 1. security_patterns.json (30KB)
정적 코드 분석용 보안 패턴

- **JavaScript/TypeScript**: 24개 패턴
- **Python**: 32개 패턴
- **Java**: 5개 패턴
- **총 61개 패턴**

**탐지 항목**:
- SQL Injection
- XSS (Cross-Site Scripting)
- Command Injection
- Hardcoded Secrets
- Path Traversal
- Insecure Deserialization
- XXE, LDAP Injection, Template Injection 등

### 2. smart_payloads.json
동적 분석용 공격 페이로드 (향후 추가 예정)

---

## 🚀 사용 방법

### 1. 프로그램 다운로드

먼저 AI Security Scanner를 다운로드하세요:
- [웹사이트에서 다운로드](https://yourwebsite.com/pentest-agent)

### 2. 패턴 자동 다운로드

프로그램에 포함된 스크립트로 자동 다운로드:

```bash
python update_from_github.py
```

### 3. 수동 다운로드 (선택)

```bash
# 직접 다운로드
curl -O https://raw.githubusercontent.com/yourusername/security-patterns/main/security_patterns.json
curl -O https://raw.githubusercontent.com/yourusername/security-patterns/main/smart_payloads.json
```

---

## 📊 패턴 구조

```json
{
  "javascript": {
    "sql_injection": [
      {
        "pattern": "정규표현식",
        "severity": "CRITICAL",
        "title": "취약점 제목",
        "description": "상세 설명"
      }
    ],
    ...
  },
  "python": {...},
  "java": {...},
  "_metadata": {
    "last_updated": "2026-02-11T10:00:00",
    "total_patterns": 61,
    "version": "1.0"
  }
}
```

---

## 🔄 업데이트 주기

- **주요 업데이트**: 월 1회 (새로운 언어/카테고리)
- **마이너 업데이트**: 주 1회 (패턴 추가/개선)
- **긴급 패치**: 필요 시 (중요 버그 수정)

---

## 🤝 기여하기

커뮤니티 기여를 환영합니다!

### 새로운 패턴 추가

1. **Fork** 이 저장소
2. **패턴 추가** (JSON 형식)
3. **테스트** (정규표현식 유효성 검증)
4. **Pull Request** 제출

### 패턴 형식

```json
{
  "pattern": "\\b(eval|exec)\\s*\\(",
  "severity": "CRITICAL",
  "title": "Dangerous function usage",
  "description": "Detects usage of eval() or exec() which can execute arbitrary code"
}
```

### 검증 도구

```bash
python validate_patterns.py
```

---

## 📝 라이선스

MIT License - 자유롭게 사용, 수정, 배포 가능

```
Copyright (c) 2026 Your Name

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

---

## 📚 관련 링크

- **프로그램 다운로드**: [yourwebsite.com/pentest-agent](https://yourwebsite.com/pentest-agent)
- **사용 가이드**: [Documentation](https://yourwebsite.com/docs)
- **이슈 리포트**: [GitHub Issues](https://github.com/yourusername/security-patterns/issues)
- **커뮤니티**: [Discord](https://discord.gg/your-invite)

---

## 📈 통계

- **총 패턴**: 61개
- **지원 언어**: 3개 (JavaScript, Python, Java)
- **마지막 업데이트**: 2026-02-11
- **기여자**: 1명 (기여 환영!)

---

## 🙏 감사의 말

이 프로젝트는 다음 오픈소스 프로젝트들의 영향을 받았습니다:
- OWASP Top 10
- CWE (Common Weakness Enumeration)
- Semgrep Rules
- Bandit Security Linter

---

## ⚠️ 면책 조항

이 패턴들은 **교육 및 합법적인 보안 테스트 목적**으로만 사용되어야 합니다.

- ✅ 자신의 시스템 테스트
- ✅ 권한을 받은 시스템 테스트
- ❌ 무단 침입 테스트 (불법!)

---

<div align="center">

**보안은 선택이 아닌 필수입니다! 🔒**

[프로그램 다운로드](https://yourwebsite.com) | [문서](https://yourwebsite.com/docs) | [커뮤니티](https://discord.gg)

**Made with ❤️ and 🤖 AI**

</div>
