# AI-LB
AI based API Load-balancing library for Spring Cloud Gateway

AI 기반의 API 로드밸런싱 Spring Cloud Gateway 라이브러리를 만드는 것을 목표로 하고 있습니다. 

전반적인 Overview는 아래와 같습니다.

![Overview_Abstract_Design](https://user-images.githubusercontent.com/29014586/133879768-5b5949f0-eb91-43ef-90ec-aacb49448461.png)

Spring Cloud Gateway는 Training/Learning된 결과를 통하여 LB를 수행합니다. 매 API Proxy의 결과는 On-line으로 수집되고, AI model로 전달됩니다.

전달된 데이터를 바탕으로 모델은 계속해서 Training을 실시하게 됩니다. Training 결과는 주기적으로 업데이트 됩니다.
