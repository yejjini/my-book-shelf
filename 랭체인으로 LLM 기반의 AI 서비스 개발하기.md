# my-book-shelf
1.1 LLM 개념
'Large language Model' -인간의 언어를 처리하는 모델.
Language Model은 새로 만들어진 것이 아니라 진화해옴.

진화과정 : 통계적 -> 신경망 언어 모델 -> 트렌스포머 -> 거대 언어모델 (LLM)

1. 통계적 - 확률 통계적 방법 기반 얼마나 자주 나오는지
   1-gram(unigram) , 2-gram(bygram) , 3-gram(trigram)
   
2. 신경망 - input layer(데이터 받아들여), hidden layer(데이터 처리), output layer(최종결과 생성)로 구성 and its all connected  and has its own diverse neuron(node).
   RNN(recurrent neural networks)- 과거의 정보가 현재에 영향을 미침, 공간이 적기 때문에 긴데이터 처리 한계
   LSTM(long short-term memory networks) - improve version of rnn , 긴 시퀀스 정보 기억 delete and undate possible
   
3. TRANSFORMER - 문장과 단락 전체 처리 가능
   BERT (bidirectional encoder representations from transformers)-양방향으로 텍스트를 분석해서 더욱더 자연스럽고 정확한 의미 파악 가능.
   GPT(gernerative pretrained transformer)- openai 개발

finally LLM - 대규모 데이터로 훈련된 큰 규모의 인공지능 기반 언어모델 ex) gpt, gemini , turbo
Parameter- 파라메터의 수로 모델의 크기를 측정 
-인터넷의 방대한 양의 텍스트 데이터로 부터 학습
-언어를 이해 생성 특화 
-특정작업을 위해 파인튜닝(fine-tuning)
-훈련 위해 상당한 컴퓨팅 지원 필요 GPU(graphic processing unit) , TPU(tensor processing unit) 하드웨어 필요 


1.2 LLM 특정과 종류




1.3 LLM 생성 과정




1.4 LLM 생성 후 추가 고려사항



2.1 LLM 활용방법



2.2 LLM 활용시 주의사항







3.2 RAG 구현 과정





3.3 RAG 구현시 필요한 것






