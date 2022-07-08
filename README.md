# BERT_skt-lecture 1
# 1. 자연어 처리(Natural language Processing, NLP)

### 1) 자연어란? 일상에서 쓰는 모든 언어
- 자연어 처리란? 자연어를 컴퓨터가 해독하고 그 의미를 이해하는 기술
(수신자가 메시지를 decoding 하는 과정)
- 다양한 자연어 처리 기술
  - symbolic approach: 패턴을 만듦 ex. (now)(weather)(what)
  - statistical approach: 확률/통계 기반 접근법 via TF-IDF(Term freq높을 수록 중요단어- Document freq)

### 2) 자연어 처리의 단계 
- 전처리: 학습데이터로 만들기 위해
- Tokenizing: 자연어를 어떤 단위로 살펴볼 것인지 ex) WordPiece 자소단위, 형태소, 어절 등
- Lexical analysis: 어휘분석, 형태소 분석, 개체명 인식 등
- Syntactic anaysis: 구문분석
- Semantic anaysis: 의미 분석

### 3) 다양한 자연어 처리 Applications
- 문서 분류(catrgory), 오타 교정, 정보 추출(wikipedia), 음성인식결과 보정, 음성 합성 텍스트 보정(input으로 영어 들어오면 한국어로 그대로 추출), 감정분석, 챗봇)
- 자연어처리 기술이 많이 활용되면 감정분석도 하고 대답도 하는 챗봇같은 걸 만들 수 있음. 
- Bert는 기계 독해 부분에서 사용됨. <br>
뉴스에서 질문하면  QnA가능하게 됨. : HOW? 그 답변을 문서에서 실시간으로 추출 => 기계독해를 통해
- 대부분의 자연어 처리 문제는 **분류**의 문제.

### 4) 자연어 에서의 특징 추출과 분류
- 분류를 위해서는 데이터를 수학적으로 표현
    - 먼저, 분류 대상의 특징(Feature)을 파악(Feature Extraction) <br>
    -> 특징을 기준으로 분류 대상을 그래프 위에 표현 <br>
    -> 대상 간 경계를 수학적으로 나눔(Classification) <br>
    -> 특징을 기준으로 그래프에 표현 해 유사도 파악 <br>
- 예전에는 사람이 직접 특징 분류함... & 실제 문제에서는 특징 사람이 파악하기 어려움 <br>
< 기계 학습의 핵심 기술!> <br>
: 컴퓨터가 스스로 찾고(Feature extraction) +  스스로 분류(Classification) <br>

### 5) 자연어에서 특징을 어떻게 추출? Word2Vec(Word embedding)
  (1) one-hot encoding: 가장 단순한 표현으로 n개의 단어를 n차원의 벡터로 표현하는 것.
    - BUT 단점: 단어의 **의미**를 벡터 공간에 표현 불가
  (2) Word2Vec 알고리즘: 주변부의 단어를 예측하는 방식으로 학습(Skip-gram방식)
    - `input(one-hot vector) + hidden layer + output` 구성
    - 자연어(단어)의 의미를 벡터 공간에 임베딩
    - 단어에 대한 dense vector을 얻을 수 있음
    - 단어의 주변 단어를 통해 그 의미를 파악할 수 있음
    - 컴퓨터에게 언어는 그저 <기호>일 뿐--> 해당 단어가 무슨 뜻인지는 모르지만, 주변 단어 형태가 비슷하니 의미도 비슷한 것이다!












2. 언어모델 (LM)




4. BERT 소개
