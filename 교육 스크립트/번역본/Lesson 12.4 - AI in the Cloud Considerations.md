## **Lesson 12.4: 클라우드에서의 AI 고려 사항**

### **강의 개요**

이 단원에서는 **클라우드에서 AI를 배포할 때 고려해야 할 여러 가지 요소**를 탐구합니다. AI 성숙도 모델을 이해하고, 조직이 이 모델의 어느 단계에 있는지 파악하는 것이 중요합니다. 이를 통해 클라우드 전략이 AI 역량과 목표에 부합하도록 결정할 수 있습니다.

### **학습 목표**

이 단원을 마치면 다음을 수행할 수 있습니다:

- **AI 성숙도 모델의 이해 및 조직의 위치 평가**: 조직의 현재 AI 역량 수준을 파악합니다.
- **온프레미스(온프렘)에서 AI를 배포할 때의 고려 사항 이해**: 온프레미스 배포의 장단점을 이해합니다.
- **클라우드에서 AI를 시작할 때의 고려 사항 이해**: 클라우드 기반 배포의 이점과 한계를 파악합니다.
- **클라우드와 온프레미스 간의 균형 잡힌 접근 방식의 필요성 인식**: 하이브리드 접근 방식의 중요성을 이해합니다.
- **AI 배포 시 주요 고려 사항 요약**: 데이터 위치, 데이터 주권, 하이브리드 IT 전략, 실시간 성능 등의 요소를 요약합니다.

---

### **핵심 내용 분석**

#### **1. AI 성숙도 모델**

AI 성숙도 모델은 조직의 AI 역량 수준을 평가하는 프레임워크로, 총 **5단계**로 구성되어 있습니다:

1. **인식(Awareness)**:
   - 조직은 AI의 잠재적 이점과 과제를 탐색하기 시작합니다.
   - 초기 대화와 실험이 있을 수 있지만, 공식적인 AI 전략이나 투자는 없습니다.

2. **활성 AI 실험(Active AI Experimentation)**:
   - 조직은 데이터 사이언스 컨텍스트에서 AI를 적극적으로 실험합니다.
   - 소규모 데이터 사이언티스트와 엔지니어 팀이 존재하지만, AI는 아직 전사적으로 퍼져 있지 않습니다.

3. **운영적 AI 생산(Operational AI in Production)**:
   - 조직은 AI를 생산 환경에 성공적으로 구현하고 프로세스를 자동화하고 의사 결정을 개선합니다.
   - AI 개발 및 배포를 위한 모범 사례가 확립되어 있으며, 다양한 AI 기술과 전문가에 접근할 수 있습니다.

4. **체계적 AI(Systemic AI)**:
   - 조직은 AI를 디지털 전략에 완전히 통합하고 혁신과 성장을 촉진합니다.
   - AI는 모든 새로운 디지털 프로젝트의 핵심 구성 요소로 간주되며, 명확한 AI 로드맵과 전략이 있습니다.

5. **변혁적 AI(Transformational AI)**:
   - AI는 조직의 DNA에 깊이 스며들어 있으며, 비즈니스 전략과 운영의 핵심 동인입니다.
   - 강력한 AI 문화가 있으며, 제품 개발부터 고객 서비스까지 비즈니스의 모든 측면에 AI가 완전히 통합되어 있습니다.

**이 모델을 사용하여 조직의 현재 AI 성숙도 수준을 평가하면**, 개선해야 할 영역을 식별하고 비즈니스 성장과 성공을 촉진하기 위한 AI 역량 발전 로드맵을 개발할 수 있습니다.

#### **2. 온프레미스에서의 AI 고려 사항**

- **자본 비용(CapEx) vs 운영 비용(OpEx)**:
  - 자체 장비를 보유하면 클라우드의 예약 인스턴스에 대한 지속적인 비용보다 총 소유 비용(TCO)이 더 유리할 수 있습니다.
  - 이는 초기 투자(CapEx)를 통해 장기적인 비용 절감을 추구하는 전략입니다.

- **데이터 주권 및 규제 준수**:
  - 데이터 센터 내에서 데이터를 유지함으로써 데이터 주권을 보장하고 규제 요구 사항을 준수할 수 있습니다.
  - 이는 보안과 컴플라이언스 측면에서 중요한 고려 사항입니다.

- **빠른 자원 활용**:
  - 온프레미스 AI를 통해 자원을 신속하게 할당하고 해제하여 AI 개발 사이클을 가속화할 수 있습니다.
  - 예측 가능한 비용 구조를 통해 예산 계획이 용이합니다.

#### **3. 클라우드에서 AI를 시작할 때의 고려 사항**

- **유연한 확장성**:
  - 클라우드 기반 AI 서비스를 통해 자원을 탄력적으로 조절하여 변화하는 요구 사항에 대응할 수 있습니다.
  - 고정된 온프레미스 인프라에 제한받지 않습니다.

- **진입 장벽 최소화**:
  - 모든 클라우드 제공업체는 NVIDIA GPU 인스턴스를 제공하며, 쉽게 활성화하고 비활성화할 수 있습니다.
  - 이는 AI 여정의 초기 단계에서 생산적인 AI 애플리케이션을 실험하는 조직에 이상적입니다.

- **운영 비용 증가 가능성**:
  - AI 역량이 성숙해짐에 따라 클라우드의 운영 비용(OpEx)이 증가할 수 있습니다.
  - 모델과 데이터셋이 커지면 더 많은 자원이 필요하게 되어 비용이 상승할 수 있습니다.

#### **4. 클라우드와 온프레미스 간의 균형 잡힌 접근 방식**

- **하이브리드 접근의 필요성**:
  - AI 워크로드에 대해 클라우드와 온프레미스 인프라를 모두 활용하는 하이브리드 접근 방식이 필요합니다.
  - 초기에는 클라우드에서 실험을 시작하고, 규모가 커지면 온프레미스로 전환하여 생산 규모의 AI 애플리케이션을 지원할 수 있습니다.

- **데이터 중력(Data Gravity)의 영향**:
  - 데이터와 컴퓨팅 자원 간의 물리적 거리는 지연 시간을 증가시키고 성능에 영향을 줍니다.
  - 예를 들어, 데이터와 클라우드 간 거리가 60마일 증가할 때마다 지연 시간이 1밀리초 증가합니다.

- **온프레미스의 보안 인식**:
  - 대규모 기업의 IT 의사 결정자의 62%는 온프레미스 보안이 클라우드 보안보다 강력하다고 믿습니다.

#### **5. 하이브리드 AI 배포의 사례**

- **훈련, 커스터마이징, 최적화의 온프레미스 수행**:
  - 훈련 환경에 대한 완전한 통제.
  - 데이터 민감성 및 규제 준수 유지.
  - 데이터 중력에 따른 정렬로 지연 시간 감소 및 성능 향상.

- **클라우드에서의 추론(Inference) 배포**:
  - 클라우드 인프라의 확장성과 유연성을 활용하여 추론 단계의 가변적인 워크로드를 효율적으로 처리합니다.

- **하이브리드 접근의 이점**:
  - 온프레미스와 클라우드 인프라의 강점을 모두 활용하면서 각자의 약점과 위험을 최소화합니다.

#### **6. AI 배포 시 주요 고려 사항 요약**

- **데이터 위치(Data Locality)**:
  - 네트워크 혼잡을 최소화하고 애플리케이션 성능을 향상시키기 위해 컴퓨팅을 데이터가 위치한 곳에 가깝게 이동시킵니다.

- **데이터 주권(Data Sovereignty)**:
  - 데이터가 생성된 지리적 위치에서 저장 및 처리되어야 한다는 국가별 요구 사항을 준수합니다.

- **하이브리드 IT 전략**:
  - AI PoC, 훈련, 대규모 배포를 위해 최상의 솔루션을 활용하기 위한 하이브리드 클라우드, 멀티 클라우드 접근 방식의 성장.

- **실시간 성능**:
  - 센서에서 생성된 데이터 기반으로 실시간 응답 또는 실시간 분석 및 인사이트를 제공해야 하는 애플리케이션 지원.
