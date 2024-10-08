## **Lesson 10: 에너지 효율적인 컴퓨팅**

### **강의 개요**

이 단원에서는 **데이터 센터에서의 에너지 효율적인 컴퓨팅**에 대해 다룹니다. 데이터 센터의 계획과 배포 단계, 전력 소비와 냉각 고려 사항, NVIDIA의 에너지 효율을 위한 기술 설계 및 최적화, 효율적인 냉각 시스템을 통한 데이터 센터의 영향 완화, 그리고 데이터 센터 콜로케이션이 효율성에 미치는 영향 등을 살펴봅니다.

### **학습 목표**

이 단원을 마치면 다음을 수행할 수 있습니다:

- 데이터 센터의 설계와 계획 단계, 그리고 설치될 장비를 포함한 전반적인 과정을 명확하게 설명할 수 있습니다.
- NVIDIA의 방법과 서버가 데이터 센터에서 에너지 효율성을 어떻게 최적화하는지 논의할 수 있습니다.
- GPU의 냉각 아키텍처가 효율성을 향상시키는 방법을 설명할 수 있습니다.
- 콜로케이션이 효율성을 어떻게 향상시키는지 이해할 수 있습니다.

---

### **핵심 내용 분석**

#### **1. 데이터 센터의 계획과 배포**

- **다섯 가지 프로세스 도메인의 균형**:

  - **데이터 센터 운영**
  - **IT 운영**
  - **NOC(Network Operations Center) 지원**
  - **애플리케이션 소유자**
  - **네트워크 운영**

- **자원 분류**: 데이터 센터 자원은 **전력**, **냉각**, **공간**으로 분류됩니다. 이들 자원은 한정되어 있으며, 하나의 변화는 다른 두 가지에 영향을 미칩니다.
- **효율성 최적화 필요성**: 자원 활용을 최적화하여 데이터 센터의 효율성을 높여야 합니다.

#### **2. 에너지 수요 증가와 GPU의 역할**

- **에너지 수요 폭발적 증가**: 대규모 데이터 로드, 복잡한 데이터 모델, 극단적인 처리 능력 요구로 인해 데이터 센터의 에너지 수요가 급증했습니다.
- **가속 컴퓨팅의 효율성**:

  - **GPU 활용**: 개별 GPU는 대규모의 계산 집약적인 기능을 적은 기술과 공간으로 처리합니다.
  - **CPU 대비 이점**: GPU는 순간적으로 더 많은 전력을 소비하지만, 워크로드 실행 시간이 크게 단축되어 전체 에너지 소비는 감소합니다.
  - **멀티-인스턴스 GPU(MIG)**: GPU를 분할하여 각 파티션에서 동시에 워크로드를 실행할 수 있으며, GPU의 전력 소비를 증가시키지 않습니다.

#### **3. NVIDIA의 효율성 향상 방법**

- **공간 및 에너지 절약**: NVIDIA GPU를 사용하는 데이터 센터는 기존 CPU 기반 시스템 대비 공간과 에너지의 일부만 필요합니다.
- **소프트웨어 최적화**:

  - **CUDA-X 라이브러리 및 GPU 가속 애플리케이션 최적화**: 동일한 GPU 아키텍처에서 성능 향상을 이룹니다.
  - **Ampere 아키텍처의 향상**: 지난 2년간 AI 워크로드가 2.5배 향상되었습니다.
  - **NGC 포털 제공**: 최신 AI 및 HPC 소프트웨어를 제공하여 성능을 향상시킵니다.
  - **에너지 절약 효과**: 성능 제안을 구현하여 NGC 워크로드에서 약 20%의 에너지 절약을 달성합니다.

- **DPU의 활용**:

  - **CPU 부담 경감**: DPU는 CPU로부터 일부 프로세스를 오프로딩하여 CPU의 부담을 30% 이상 감소시킵니다.
  - **성능 향상**: 일부 워크로드에서 50배 이상의 성능 향상을 달성하여 서버 수를 줄이고 전력을 절감합니다.
  - **보안 강화**: NVIDIA DPU가 지원하는 제로 트러스트 보호 플랫폼은 데이터 센터에 새로운 수준의 보안을 제공하며, 인프라와 전력 요구량을 더욱 줄여줍니다.

- **네트워킹 효율성**:

  - **NVIDIA Spectrum-4 Ethernet 스위치**: 이전 세대 대비 40% 낮은 전력 소비로 극한의 네트워킹 성능과 강력한 보안을 제공합니다.

#### **4. 냉각 시스템과 효율성**

- **냉각의 중요성**: 슈퍼컴퓨터의 성능을 최적화하려면 적절한 냉각이 필수적입니다.
- **NVIDIA의 냉각 기술**:

  - **CFD 모델 사용**: 데이터 센터 설계와 서버 랙 배치에서 계산 유체 역학 모델을 사용하여 냉각을 향상시킵니다.
  - **PINN 활용**: NVIDIA Modulus의 물리 정보 뉴럴 네트워크를 사용하여 DGX 시스템의 히트싱크를 설계합니다.
  - **냉각 솔루션 최적화**: 서버 랙과 밀접하게 결합하여 열 전달을 지역화하고 최적화합니다.
  - **레퍼런스 아키텍처 제공**: 최적의 DGX 서버 제품 배포를 위한 레퍼런스 아키텍처를 제공하여 고객과 파트너가 배포를 최적화하도록 돕습니다.

#### **5. 가속 컴퓨팅의 에너지 효율성**

- **효율성 지표**: 애플리케이션 처리량 대비 킬로와트시(kWh)로 에너지 효율성을 측정합니다.
- **성능 비교**:

  - **HGX H100 4x GPU 시스템 vs. 듀얼 소켓 Sapphire Rapids 시스템**: GPU 시스템은 22.9배의 성능 이점을 가집니다.
  - **에너지 소비 비교**: 50노드 HGX 슈퍼컴퓨터는 연간 2.6기가와트시를 사용하며, CPU 시스템은 1,150대의 서버로 12.1기가와트시를 사용합니다.
  - **결론**: 가속화된 플랫폼은 큰 에너지 효율성 이점을 제공합니다.

#### **6. 데이터 센터 냉각과 NVIDIA의 최적화**

- **GPU의 열 방출**:

  - **GPU 칩 전력 소비**: 250-500와트로 작동하여 열을 크게 증가시킵니다.
  - **랙의 열 출력 증가**: GPU 랙의 열 출력은 12킬로와트에서 45킬로와트에 이릅니다.

- **냉각 옵션**:

  - **냉각 공기**: 저렴하지만 랙당 30킬로와트의 냉각에 한계가 있습니다.
  - **수냉식 열교환기**: 더 효율적이지만 비용이 높으며, 랙당 20-60킬로와트를 처리할 수 있습니다.

- **냉각 시스템 구현**:

  - **직접 공기 냉각 시스템**: CRAH(Computer Room Air Handling Units)를 사용하여 찬 공기를 순환시키고, 시스템 팬이 찬 공기를 흡입하여 열을 제거합니다.
  - **열 방출을 위한 수냉식 옵션**: 서버와 가까운 후면 도어에 냉각 코일을 배치하여 효율적으로 열을 제거합니다.

#### **7. 데이터 센터 콜로케이션의 이점**

- **콜로케이션 필요성**: 일부 기업은 가속 컴퓨팅을 지원할 수 있는 현대적인 데이터 센터 시설이 없습니다.
- **NVIDIA DGX-ready 데이터 센터 프로그램**:

  - **파트너 제공**: NVIDIA 파트너가 제공하며, 아시아, 호주, 유럽, 북미, 남미에서 이용 가능합니다.
  - **이점**: 시설 계획의 어려움이나 퍼블릭 클라우드의 높은 비용과 지연을 피하고, 데이터에서 인사이트를 얻고 혁신에 집중할 수 있습니다.
  - **서비스 확장**: 일부 파트너는 테스트 드라이브 및 GPU as a Service 등 더 광범위한 서비스를 제공합니다.

#### **8. NVIDIA의 넷 제로 데이터 센터 목표**

- **지속적인 개선 노력**: GPU 하드웨어와 네트워킹 장비 전반에서 개선을 통해 넷 제로 데이터 센터를 추구합니다.
- **아키텍처 전환의 이점**: Ampere에서 Hopper로의 전환에서 상당한 개선이 있었으며, AI 워크로드를 더 빠르고 효율적으로 실행하여 GPU 사용 시간이 감소합니다.
- **예시**: Ampere GPU 아키텍처는 TF32 수학 모드를 도입하여 FP32 훈련과 동일한 정확도로 딥러닝 훈련을 가속화합니다.