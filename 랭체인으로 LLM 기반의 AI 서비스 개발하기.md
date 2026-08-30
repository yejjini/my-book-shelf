# my-book-shelf
1.1 LLM 개념
'Large language Model' -인간의 언어를 처리하는 모델.
Language Model은 새로 만들어진 것이 아니라 진화해옴.

진화과정 : 통계적 -> 신경망 언어 모델 -> 트렌스포머 [거대 언어모델 (LLM)]

1. 통계적 - 확률 통계적 방법 기반 얼마나 자주 나오는지
   1-gram(unigram) , 2-gram(bygram) , 3-gram(trigram)
   
2. 신경망 - input layer(데이터 받아들여), hidden layer(데이터 처리), output layer(최종결과 생성)로 구성 and its all connected  and has its own diverse neuron(node).
   RNN(recurrent neural networks)- 과거의 정보가 현재에 영향을 미침, 공간이 적기 때문에 긴데이터 처리 한계
   LSTM(long short-term memory networks) - improve version of rnn , 긴 시퀀스 정보 기억 delete and undate possible

LLM - 대규모 데이터로 훈련된 큰 규모의 인공지능 기반 언어모델 ex) gpt, gemini , turbo
Parameter- 파라메터의 수로 모델의 크기를 측정 
Prompt 입력  - completion 답변 형태

3. TRANSFORMER - 문장과 단락 전체 처리 가능, LLM 의 기본 모델
   BERT (bidirectional encoder representations from transformers)-양방향으로 텍스트를 분석해서 더욱더 자연스럽고 정확한 의미 파악 가능.
   GPT(gernerative pretrained transformer)- openai 개발


1.2 LLM 특정과 종류 

-인터넷의 방대한 양의 텍스트 데이터로 부터 학습
-언어를 이해 생성 특화 
-특정작업을 위해 파인튜닝(fine-tuning)
-훈련 위해 상당한 컴퓨팅 지원 필요 GPU(graphic processing unit) , TPU(tensor processing unit) 하드웨어 필요 

LLM의 생태계 
-Infrastructure layer : NVIDIA , OPEN AI , HUGGING FACE , GOOGLE , MS -> NEED TO FOCUS ON INFERENCE PART
-application layr : 프레임워크와 서비스로 활용할 수 있는 BI TOOL 제공 회사들이 포함

종류 
GPT-4 : multimodal 제공 , 보고 듣기 같이 가능 
팜2 : gpt-4 랑 언어모델 제공 기능 일치 but 데이터 크키가 좀 더 작을 것 예측 
라마2 : 오픈 소스로 공개 상업적 x 라는 강점 , slm 도 제공 

생성형 AI = GAI ( generative AI) VS LLM 
LLM 은 언어(text) 중심 생성형 AI 는 입력 데이터 기반으로 새로운걸 생성 
-> GAI > LLM

SLM vs LLM 
SLM 특정 분야에 특화된 단순작업만 동작 LLM 배포 어렵 복잡한 직업 처리 가능 

1.3 LLM 생성 과정

1. 데이터 수집 및 준비 : 데이터 수집, 정제, 전처리 (tokenization : 텍스트 작은단위로 나누는 과정, 정규화 ) , 형식 변경 
2. 모델 설계 : 매우 큰 신경망 아키텍처 구축, hyperparameter 설정 
3. 모델 학습 : modeling ( 만들어진 내부적인 패턴이나 규칙)
4. 평가 및 검증 
5. 배포 및 유지 보수


2.1 LLM 활용방법
파인튜닝(Fine-tuning) : 기존 LLM 특정 작업이나 상황에 맞게 더 훈련시킨 과정 
RAG ( Retrieval-Augmented Generation) : retrieval <-> generation 정보 검색과 생성을 결합한 인공지능 모델 , 복잡한 정보 질문 대답하기 위해 설계됨
-> 파인튜닝보다 RAG 선호 

비슷한 걸로 few shot learning , zero shot learning , one shot learning 있음 . 데이터의 양에 따라 나뉨.


2.2 LLM 활용시 주의사항
1. 정보 필터링
2. 법적인 규제
3. 할루시네이션(Hallucination): 언어모델이 부정확하거나 관련없는 정보를 생성하는 현상.  -> temperature 사용을  hallucination 방지
4. 보안


3.1 RAG 개념, 구현 과정
RAG ( Retrieval-Augmented Generation)- llm 에서 인터넷 정보가 필요할 때 그 정보를 가져다 텍스트로 바꿔주는거 

1. 정보 검색 : 질문 입력 (query) ,

   
3. 텍스트 생성






3.2 RAG 구현시 필요한 것






