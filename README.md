# Ansible 실습 및 GitHub 업로드 자동화

## 실습 환경
- CentOS VMware VM
- VS Code Remote SSH
- Git 및 Ansible

## 저장소 내용
Ansible 인벤토리, 변수, Vault, 조건문, 반복문,
핸들러, 템플릿 등의 실습 파일을 포함합니다.

## GitHub 업로드 자동화
upload.yml은 Git 저장소 초기화, 원격 저장소 연결,
변경 감지, 커밋 및 GitHub 푸시를 수행합니다.

## 사전 준비
GitHub에 빈 저장소를 만들고 SSH 공개키를 등록합니다.
upload.yml의 저장소 주소와 작성자 정보를 수정합니다.

## 실행
```bash
ansible-playbook -i localhost, upload.yml
```

변경 사항이 있을 때만 새 커밋을 생성합니다.