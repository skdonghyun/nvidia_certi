## **Lesson 12.6: 클라우드에서의 NVIDIA 솔루션**

### **강의 개요**

이 단원에서는 **NVIDIA의 클라우드 기반 AI 솔루션**과 이러한 솔루션이 클라우드에서 AI의 강력한 기능을 활용하는 데 어떻게 도움이 되는지를 탐구합니다.

### **학습 목표**

이 단원을 마치면 다음을 수행할 수 있습니다:

- **NVIDIA AI 플랫폼의 이해**: NVIDIA AI 플랫폼이 엔터프라이즈 AI의 과제를 어떻게 해결하고, 고객의 위치에 맞춰 어떻게 대응하는지 이해합니다.
- **클라우드에서 NVIDIA 기술 활용 방법 파악**: NVIDIA AI 플랫폼의 각 계층에서 클라우드 고객을 위한 NVIDIA 기술 소비 방법을 이해합니다.
- **NVIDIA의 클라우드 솔루션 분석**: NVIDIA AI Enterprise, NGC, DGX Cloud, NVIDIA AI Foundations, NVIDIA AI Foundry 등 NVIDIA의 클라우드 솔루션을 이해하고, 워크로드에 어떻게 도움이 되는지 평가합니다.

---

### **핵심 내용 분석**

#### **1. NVIDIA AI 플랫폼 소개**

- **전체 스택 플랫폼**: NVIDIA AI 플랫폼은 엔터프라이즈 AI의 과제를 해결하고, 고객이 AI 채택 여정에서 어디에 있든 비즈니스 결과를 제공할 수 있도록 설계되었습니다.
- **클라우드 네이티브**: NVIDIA AI 플랫폼은 클라우드 네이티브로 설계되어, 퍼블릭 클라우드, 엔터프라이즈 데이터 센터, 엣지 위치 등 어디에서나 AI 애플리케이션을 개발하고 배포할 수 있습니다.
- **클라우드 락인 방지**: 특정 클라우드나 배포 옵션에 종속되지 않으므로 유연하게 활용할 수 있습니다.

#### **2. NVIDIA AI 플랫폼의 계층별 분석**

- **가장 하단 계층: 가속화된 인프라스트럭처**

  - **가상 머신 인스턴스(VMI)**: NVIDIA GPU를 탑재한 가상 머신 인스턴스.
  - **NVIDIA 가상 머신 이미지(VMI)**: CSP 마켓플레이스를 통해 제공되며, NVIDIA GPU 가속 소프트웨어를 실행하기 위한 운영 체제 환경을 제공합니다.
    - **Ubuntu OS 기반**으로 구축되고, 핵심 종속성을 패키징합니다.
    - **GPU 최적화된 개발 환경**을 제공합니다.
  - **클라우드 인스턴스 유형**: CSP가 제공하는 사전 정의된 가상 서버 구성으로, CPU, 메모리, 스토리지, 네트워킹 등의 리소스를 지정합니다.

- **중간 계층: AI 플랫폼 소프트웨어 계층**

  - **NVIDIA AI Enterprise**
    - **엔터프라이즈 AI 애플리케이션을 위한 클라우드 네이티브 AI 소프트웨어 플랫폼**.
    - **생산 환경의 AI 워크로드**를 위해 설계되었으며, 퍼블릭, 하이브리드, 멀티 클라우드 등 다양한 배포 환경에서 사용할 수 있습니다.
    - **최적화된 성능**: 가속화된 인프라스트럭처의 성능을 최대한 활용하여 운영 비용을 절감합니다.

- **상위 계층: NVIDIA NGC 카탈로그**

  - **중앙 허브 역할**: NVIDIA의 서비스, 소프트웨어, 지원을 위한 중앙 허브로, AI 제공을 위한 원스톱 숍입니다.
  - **NVIDIA AI Enterprise와의 연계**: NVIDIA AI Enterprise의 구독이나 라이선스를 통해 NGC에서 엔터프라이즈 카탈로그에 접근하여 AI 워크플로우와 새로운 AI 서비스를 이용할 수 있습니다.
  - **무료 소프트웨어 접근과의 차이점**: NGC를 통한 무료 소프트웨어 접근은 NVIDIA AI Enterprise가 제공하는 엔터프라이즈 지원, SLA, NVIDIA AI 전문가의 접근, 독점적인 엔터프라이즈 제품 차별화 요소 등을 제공하지 않습니다.

- **최상위 계층: AI 서비스 계층**

  - **NVIDIA의 최신 클라우드 포트폴리오 추가 요소**로, 고객이 플랫폼과 상호 작용할 수 있는 가장 높은 수준의 추상화 계층입니다.
  - **NVIDIA가 관리하는 서비스로서의 가치 제공**: 전체 NVIDIA AI 플랫폼의 가치를 엔드 고객에게 제공합니다.

#### **3. NVIDIA의 클라우드 솔루션 상세 분석**

- **NVIDIA DGX Cloud**

  - **멀티노드 AI 트레이닝 서비스**: 엔터프라이즈 AI를 위한 서비스로, 대규모 모델 훈련에 적합합니다.
  - **올인원 월간 가격**으로 제공되며, NVIDIA Base Command Platform, NVIDIA AI Enterprise 소프트웨어, NVIDIA DGX 인프라스트럭처, NVIDIA AI 전문 지식 및 지원에 대한 접근을 포함합니다.
  - **브라우저 기반 시작**: 고객은 자체적으로 AI 슈퍼컴퓨터를 조달, 설정, 관리할 필요 없이 브라우저만 열어서 시작할 수 있습니다.
  - **여러 퍼블릭 클라우드에서 호스팅**: Oracle Cloud Infrastructure, Microsoft Azure, Google Cloud 등에서 제공됩니다.

- **NVIDIA AI Foundations**

  - **NVIDIA DGX Cloud를 기반으로 하는 NVIDIA 관리 클라우드 서비스 모음**.
  - **맞춤형 생성 AI 구축 및 실행을 위한 클라우드 서비스**로, 텍스트 언어, 시각 미디어, 생물학을 위한 최첨단 파운데이션 모델을 활용합니다.
  - **두 가지 컬렉션 포함**:
    - **NeMo 모델**: 책임감 있게 소싱된 데이터를 사용하여 훈련된 엔터프라이즈 준비 모델.
      - **50개 이상의 언어와 35개의 코딩 언어 지원**.
      - **다양한 산업에서의 적용**: 의료, 통신, 금융 서비스 등.
    - **커뮤니티 모델**: NVIDIA가 최적화한 모델로, LLAMA 2, Mistral, Stable Diffusion, Code Llama 등이 포함됩니다.
      - **TensorRT LLM을 사용하여 최적의 성능 효율성 달성**.
      - **NeMo 형식으로 변환되어 커스터마이징이 용이함**.

- **NVIDIA AI Foundry**

  - **맞춤형 생성 AI 모델을 생성하기 위한 새로운 유형의 서비스**.
  - **세 가지 요소로 구성**:
    - **NVIDIA AI 파운데이션 모델**: 최첨단 사전 훈련된 모델과 NVIDIA가 최적화한 커뮤니티 파운데이션 모델.
    - **NVIDIA NeMo 프레임워크**: 엔터프라이즈급 런타임과 함께 모델을 미세 조정하기 위한 도구 제공.
    - **NVIDIA DGX Cloud**: 다양한 하이퍼스케일러에서 실행되는 엔터프라이즈 개발자를 위한 서버리스 AI 트레이닝 서비스 플랫폼.
  - **출력물**: 독점 데이터, 가드레일, 추론 런타임으로 조정된 맞춤형 모델 컨테이너.
  - **배포 유연성**: 커스터마이징된 엔터프라이즈 독점 모델은 NVIDIA AI Enterprise를 사용하여 가속 컴퓨팅에서 엔터프라이즈급 보안, 안정성, 지원으로 거의 어디서나 배포할 수 있습니다.

#### **4. NVIDIA 솔루션의 클라우드에서의 소비 방식 요약**

- **NVIDIA 가속화된 인프라스트럭처**: 클라우드에서 NVIDIA 기술을 광범위하게 사용할 수 있게 하는 기반 요소입니다.
- **전체 스택 플랫폼 제공**: 이제 클라우드에서 전체 스택 플랫폼을 소비할 수 있습니다.
  - **AI 서비스 소비**: DGX Cloud, AI Foundations, AI Foundry 등을 통한 전체 스택 소비.
  - **소프트웨어 및 인프라 소비**: NVIDIA AI Enterprise 소프트웨어와 인프라를 함께 소비.
  - **인프라 레벨의 소비**: CSP와의 통합을 통해 NVIDIA AI 플랫폼의 다양한 계층을 활용.
- **고객의 가치 창출 경로 제공**: 고객이 이미 사용 중인 클라우드 서비스 내에서도 NVIDIA를 사용하고 가치를 창출할 수 있는 경로를 제공합니다.
