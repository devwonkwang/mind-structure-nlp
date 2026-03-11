# 마음의 구조와 자연어 처리

*(The Structure of the Mind and Natural Language Processing)*

이 저장소 혹은 페이지는 조원광의 **<마음의 구조와 자연어 처리> 강의**의 강의안과 관련 자료를 모아 놓은 곳입니다.
현재 공개된 자료는 **초안 형태의 강의 노트**를 중심으로 구성되어 있습니다. 
향후 **지속적으로 수정·확장될 예정입니다.**

이 저장소는 하나의 완결된 프로젝트가 아니라, 
**연구와 교육 과정 속에서 계속 발전하는 공개 강의 자료(open educational resource)**의 성격을 갖습니다.
강의 노트, 코드 예제, 데이터 처리 과정 등이 점차 추가되며 업데이트될 예정입니다.

---

## 전체 목차 (설계도)

현재 저장소에는 일부 장만 연결되어 있으며,
아래 목차는 본 강의가 지향하는 **전체 구성의 설계도**를 보여줍니다.

---

### Part 1. 네트워크 과학을 활용한 분석

1. 서론: 마음의 구조와 자연어 처리
2. 언어를 네트워크로 바라보기
3. 네트워크 중심성을 활용한 언어 자료 분석
4. 네트워크 커뮤니티 포착 알고리즘과 언어 자료 분석
5. 토크나이저의 종류와 활용

---

### Part 2. 토픽 모델링을 활용한 분석

6. 토픽 모델링의 세계관
7. 샘플링을 통한 사후 분포 근사와 LDA 구현
8. Variational Inference를 활용한 LDA 구현
9. 토픽 모델링을 활용한 연구에서 고려할 점들

---

### Part 3. 신경망/딥러닝 모델을 활용한 분석

10. 신경망 알고리즘 기초
11. Word2Vec의 개요와 응용
12. RNN의 취지, 한계, 그리고 극복 시도들
13. 셀프 어텐션과 트랜스포머
14. GPT와 BERT를 활용한 연구 사례
15. 나가며: 세 가지 접근법의 장점과 한계, 그리고 마음의 구조

---

> 현재 공개된 버전에서는 일부 장만 실제로 연결되어 있습니다.
> 나머지 장들은 **향후 추가될 예정**입니다.

---

## 환경 설정 (실습 코드 실행)

이 교재의 실습 코드를 실행하려면 **conda 환경**을 사용하는 것을 권장합니다.

먼저 conda의 solver를 빠른 방식으로 설정합니다.
(이 작업은 처음 한 번만 실행하면 됩니다.)

```
conda config --set solver libmamba
conda config --set channel_priority strict
```

그 다음 아래 환경 중 하나를 생성합니다.

### 기본 환경 (Part 1–2)

```
conda env create -f environment-core.yml
```

### 딥러닝 CPU 환경 (Part 3)

```
conda env create -f environment-deep-cpu.yml
```

### 딥러닝 GPU 환경 (Part 3, GPU 사용 가능 시)

```
conda env create -f environment-deep-gpu.yml
```

환경 생성 후에는 예를 들어 다음과 같이 활성화할 수 있습니다.

```
conda activate mind-nlp-core
```

---

## Author

**조원광 (Wonkwang Jo)**
Seoul National University
Graduate School of Public Health

2026

---

## License

CC BY 4.0
(Creative Commons Attribution 4.0 International)

---

## AI-assisted development note

이 저장소의 일부 코드 예제, 데이터 처리 과정, 시각화 자료 등은 **ChatGPT (OpenAI)**의 도움을 받아 작성되었습니다.

정보 검색 및 초고 작성 후 내용 검토를 위해서도 **ChatGPT (OpenAI)**가 보조 도구로 활용되었습니다. 

모든 내용은 **조원광(Wonkwang Jo)**이 검토하고 최종 수정한 것입니다.