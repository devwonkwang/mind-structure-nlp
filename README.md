# 마음의 구조와 자연어 처리

*(The Structure of the Mind and Natural Language Processing)*

**공개 초안 v0.1 (2026년 3월)**

이 프로젝트는 조원광의 **<마음의 구조와 자연어 처리>** 의 강의안과 관련 자료를 모아 놓은 것입니다.  
현재 공개된 자료는 **교재 초안 형태의 강의안**을 중심으로 구성되어 있습니다.  
이 강의안들은 독자가 처음부터 끝까지 혼자 읽어가면서 이론적 이해를 습득하고 실습을 진행할 수 있도록 구성되었습니다.  
향후 **지속적으로 수정하고 확장할 예정입니다.**


이 프로젝트는 계획된 장을 추가하고 이미 있는 강의안들을 수정 보완하여,  
향후 <마음의 구조와 자연어 처리>(가제)라는 공개 전자책 교재로 확장하는 것을 목표로 합니다.  
현재 공개된 강의안들은 이 책의 미완성 초고인 셈입니다.  
물론 향후 공개 전자책으로 변화해도, 지금처럼 모든 글과 자료가 접근 가능하도록 유지할 것입니다. 


이 강의안 혹은 교재 초안은 인문사회과학 개념과 자연어 처리의 연결을 시도하고 있습니다.  
양쪽 모두에 관심있는 독자들에게 유익한 자료가 될 것이라 예상합니다.  
동시에 독자들이 자연어 처리 기법의 수학적 원리를 파악할 수 있도록,  
난이도를 타협하지 않되 접근 가능한 설명을 제시하려고 노력했습니다.  


이 프로젝트는 완결된 결과가 아니라, **연구와 교육 과정 속에서 계속 발전하는 공개 강의 자료(open educational resource)** 의 성격을 갖습니다.  
코드 예제, 데이터 처리 과정 등이 점차 추가될 것이며 강의안의 내용 또한 수정 보완될 것입니다.  
이 강의 자료의 원본 노트북, 환경 파일, 설정 파일은 아래 GitHub 저장소에서 확인할 수 있습니다.


이 프로젝트의 웹 버전은 아래에서 확인할 수 있습니다:  
https://devwonkwang.github.io/mind-structure-nlp/

GitHub 저장소는 아래와 같습니다:  
https://github.com/devwonkwang/mind-structure-nlp

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
9. 토픽 모델링을 활용한 연구에서 고려할 점들 (추가 예정)

---

### Part 3. 신경망/딥러닝 모델을 활용한 분석

10. 신경망 알고리즘 기초
11. Word2Vec의 개요와 응용 (추가 예정)
12. RNN의 취지, 한계, 그리고 극복 시도들 (추가 예정)
13. 셀프 어텐션과 트랜스포머 (추가 예정)
14. GPT와 BERT를 활용한 연구 사례 (추가 예정)
15. 나가며: 세 가지 접근법의 장점과 한계, 그리고 마음의 구조 (추가 예정)

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

© Wonkwang Jo  

CC BY-SA 4.0  
(Creative Commons Attribution-ShareAlike 4.0 International)

이 자료는 Creative Commons Attribution-ShareAlike 4.0 International 라이선스에 따라 배포됩니다.  
자세한 내용은 다음을 참고하십시오:  
https://creativecommons.org/licenses/by-sa/4.0/

---

## AI-assisted development note

이 저장소의 일부 코드 예제, 데이터 처리 과정, 시각화 자료 등은 **ChatGPT (OpenAI)** 의 도움을 받아 작성되었습니다.

정보 검색 및 초고 작성 후 내용 검토를 위해서도 **ChatGPT (OpenAI)** 가 보조 도구로 활용되었습니다. 

모든 내용은 **조원광(Wonkwang Jo)** 이 검토하고 최종 수정한 것입니다.