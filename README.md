# Sentinel 정책 디렉토리

## 개요

이 디렉토리는 HashiCorp Sentinel 정책 파일을 관리하기 위한 공간입니다.  
Sentinel은 HashiCorp 제품(Terraform, Vault, Consul 등)에서 정책 기반의 접근 제어와 거버넌스를 구현할 수 있는 정책 엔진입니다.

## 사용 목적

- Terraform 실행 시 인프라 변경에 대한 정책 검증
- 조직의 보안 및 컴플라이언스 요구사항 준수
- 인프라 리소스 생성, 변경, 삭제에 대한 세부 제어

## 예시 구조

```
sentinel/
├── restrict-iam-policy-statement.sentinel
├── sentinel.hcl
└── README.md
```

## 주요 정책 예시

- **restrict-iam-policy-statement.sentinel**  
  IAM 정책의 Statement를 제한하는 예시 정책

## 적용 방법

1. Sentinel 정책 파일을 이 디렉토리에 추가합니다.
2. HCP Terraform 또는 Terraform Enterprise에서 Sentinel 정책을 연결하여 적용합니다.

## 참고 자료

- [Sentinel 공식 문서](https://docs.hashicorp.com/sentinel/)
- [Terraform Sentinel 통합](https://docs.hashicorp.com/terraform/cloud/sentinel/)
