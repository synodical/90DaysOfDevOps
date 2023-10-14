## The Big Picture: DevSecOps 큰 그림: DevSecOps(데브섹옵스)

2023년 에디션의 두 번째 날인 오늘, 이 첫 번째 모듈에서는 DevSecOps에 대한 기본 개요를 살펴보려 합니다.

### What is DevSecOps? DevSecOps란 무엇인가?

DevSecOps는 개발, 보안, 운영 팀을 하나로 결합하여 안전한 소프트웨어 애플리케이션을 구축하고 유지하는 소프트웨어 개발 접근 방식입니다. 이는 지속적 통합, 지속적 전달, 지속적 배포 원칙을 기반으로 하며, 소프트웨어 업데이트와 기능을 더 빠르고 자주 제공하는 것을 목표로 합니다. DevSecOps에서 보안은 단순히 후속 조치가 아닌 소프트웨어 개발 프로세스의 핵심 부분입니다. 이는 보안 테스트, 모니터링 및 기타 보안 조치가 소프트웨어 개발 생명 주기 (SDLC)에 처음부터 포함되는 것을 의미합니다. DevSecOps는 개발, 보안 및 운영 팀 간의 협업과 커뮤니케이션을 향상시켜 보다 효율적이고 효과적인 소프트웨어 개발 프로세스를 만들기 위해 노력합니다.

### DevSecOps vs DevOps 데브섹옵스(DevSecOps) 대 데브옵스(DevOps)

여기서 "대"라는 표현은 가볍게 사용됩니다만, 2022년 에디션을 떠올려보면 데브옵스의 목표는 소프트웨어 릴리스의 속도, 신뢰성 및 품질을 개선하는 것입니다.

DevSecOps는 DevOps 철학의 확장으로, 보안 관행을 소프트웨어 개발 프로세스에 통합하는 것을 강조합니다. DevSecOps의 목표는 보안 조치를 소프트웨어 개발 프로세스에 내장하여 시작부터 보안을 소프트웨어의 핵심 부분으로 만드는 것입니다. 이는 보안 취약점이 소프트웨어에 도입되는 위험을 줄이고 발생하는 문제를 식별하고 수정하기가 더 쉬워지게 합니다.

데브옵스는 개발자와 운영 스태프 간의 협업과 커뮤니케이션을 향상시켜 소프트웨어 릴리스의 속도, 신뢰성 및 품질을 개선하는 것에 중점을 두는 반면, DevSecOps는 소프트웨어 개발 프로세스에 보안 관행을 통합하여 보안 취약점의 위험을 줄이고 소프트웨어의 전체적인 보안을 개선하는 데 중점을 둡니다.

### Automated Security 자동화된 보안

Automated security refers to the use of technology to perform security tasks without the need for human intervention. This can include things like security software that monitors a network for threats and takes action to block them, or systems that use artificial intelligence to analyse security footage and identify unusual activity. Automated security systems are designed to make security processes more efficient and effective, and to help reduce the workload on security personnel.

A key component of all things DevSecOps is the ability to automate a lot of the tasks at hand when creating and delivering software, when we add security from the start it means we also need to consider the automation aspect of security. 

자동화된 보안은 사람의 개입 없이 보안 작업을 수행하기 위해 기술을 사용하는 것을 말합니다. 이는 네트워크를 위협하고 차단 조치를 취하는 보안 소프트웨어나 보안 영상을 분석하고 비정상적인 활동을 식별하는 인공 지능 시스템과 같은 것을 포함합니다. 자동화된 보안 시스템은 보안 프로세스를 더 효율적이고 효과적으로 만들며 보안 인력의 작업 부담을 줄이는 데 도움이 됩니다.

DevSecOps의 모든 요소 중 핵심은 소프트웨어를 생성하고 전달할 때 많은 작업을 자동화할 수 있는 능력입니다. 시작부터 보안을 추가한다는 것은 보안의 자동화 측면을 고려해야 함을 의미합니다.

### Security at Scale (Containers and Microservices) 규모에 맞는 보안 (컨테이너 및 마이크로서비스)

We know that the scale and dynamic infrastructure that has been enabled by containerisation and microservices have changed the way that most organisations do business. 

This is also why we must bring that automated security into our DevOps principles to ensure that specific container security guidelines are met. 

What I mean by this is with cloud-native technologies we cannot only have static security policies and posture; our security model also must be dynamic with the workload in hand and how that is running. 

DevOps teams will need to include automated security to protect the overall environment and data, as well as continuous integration and continuous delivery processes. 

The below list is taken from a [RedHat blog post](https://www.redhat.com/en/topics/devops/what-is-devsecops)

- Standardise and automate the environment: Each service should have the least privilege possible to minimize unauthorized connections and access.

- Centralise user identity and access control capabilities: Tight access control and centralised authentication mechanisms are essential for securing microservices since authentication is initiated at multiple points.

- Isolate containers running microservices from each other and the network: This includes both in-transit and at-rest data since both can represent high-value targets for attackers.

- Encrypt data between apps and services: A container orchestration platform with integrated security features helps minimize the chance of unauthorized access.

- Introduce secure API gateways: Secure APIs increase authorization and routing visibility. By reducing exposed APIs, organizations can reduce surfaces of attacks.

대부분의 조직이 비즈니스를 수행하는 방식은 컨테이너화와 마이크로서비스의 규모와 동적 인프라 덕분에 변경되었습니다.

이것은 우리가 특정 컨테이너 보안 지침을 준수하기 위해 데브옵스 원칙에 자동화된 보안을 도입해야 하는 이유이기도 합니다.

즉, 클라우드 네이티브 기술을 사용할 때 정적인 보안 정책과 자세만 갖추는 것으로는 충분하지 않다는 것을 의미합니다. 보안 모델은 작업 부하와 실행 방식에 따라 동적이어야 합니다.

데브옵스 팀은 전체적인 개발 환경 및 데이터와, 지속적 통합 및 지속적 전달 프로세스를 보호하기 위해 자동화된 보안을 포함해야 합니다.

아래 목록은 [RedHat blog post](https://www.redhat.com/en/topics/devops/what-is-devsecops)에서 가져온 것입니다.

- 환경을 표준화하고 자동화: 각 서비스는 권한을 최소화하여 무단 연결과 액세스를 최소화해야 합니다.

- 사용자 신원 및 접근 제어 기능을 중앙 집중화: 마이크로서비스 아키텍처에서는 여러 마이크로서비스 간에 사용자 인증이 여러 지점에서 시작될 수 있습니다. 다양한 인증 지점을 효과적으로 관리하고 보호하기 위해서 강력한 접근 제어 및 중앙 집중식 인증 메커니즘이 필수적입니다.

- 마이크로서비스를 동작하게끔 하는 서로 다른 컨테이너 및 네트워크 간에 격리: 이는 in-transit과 및 at-rest 데이터 모두 포함됩니다. 양쪽 모두가 공격자에게 공격할 가치가 충분한 타겟이 될 수 있기 때문입니다.

- 앱 및 서비스 간 데이터 암호화: 통합 보안 기능이 포함된 컨테이너 오케스트레이션 플랫폼을 사용하면 인증되지 않은 액세스 가능성을 최소화할 수 있습니다.

- 안전한 API 게이트웨이 도입: 안전한 API는 승인 및 라우팅 가시성을 높입니다. 노출된 API를 줄이면 조직은 공격에 노출될만한 부분을 줄일 수 있습니다.

### Security is HOT right now 보안은 현재 매우 중요한 이슈입니다.

One thing you will have seen regardless of your background is that security is hot all over the industry, this is partly to do with security breaches appearing in global news and big brands being affected by security vulnerabilities or following potential bad practices allowing bad actors into the networks of these companies. It is fair to say or at least from my perspective the creation of software is much more achievable and obtainable now than it ever has. But in creating software it is increasingly exposed with vulnerabilities and the like which allows the bad actors to cause havoc and sometimes hold data to ransom or shut down businesses causing mayhem. We have discussed so far what is DevSecOps but I think it is also worthwhile exploring the cybersecurity side of the attack vector and why we protect our software supply chain to help avoid these cyber-attacks. 

당신이 어떤 직군이든 간에 상관없이 보안은 산업 전반에 걸쳐 핫한 주제임을 알 수 있을 것입니다. 전세계적으로 뉴스에서 보안 침해 사례가 나타나고 큰 기업들이 보안 취약점에 영향을 받거나 바람직하지 못한 보안 습관때문에 나쁜 의도를 가진 자들이 해당 회사들의 네트워크에 침입하는 경우 때문이라고 할 수 있습니다. 말하자면 이전보다 소프트웨어를 만드는 것이 훨씬 간단해진 시대가 되었다고도 할 수 있습니다. 그러나 소프트웨어를 생성하면서 취약성과 같은 문제가 점점 노출되고 있으며 이는 나쁜 의도를 가진 자들이 혼란을 일으키고 때로는 데이터를 금전적 요구 대가로 납치하거나 비즈니스를 마비시키는 것을 허용합니다. 지금까지 DevSecOps가 무엇인지 논의해 보았지만, 저는 사이버 공격 벡터의 사이버 보안 측면을 탐구하고 왜 우리가 소프트웨어 공급망을 보호하여 이러한 사이버 공격을 피하려고 하는지에 대해서도 탐구하는 것이 바람직하다고 생각합니다.

### Cybersecurity vs DevSecOps

As the heading goes it is not really a vs but more of a difference between the two topics. But I think it is important to raise this as really this will explain why Security must be part of that DevOps process, principles, and methodology. 

Cybersecurity is the practice of protecting computer systems and networks from digital attacks, theft, and damage. It involves identifying and addressing vulnerabilities, implementing security measures, and monitoring systems for threats.

DevSecOps, on the other hand, is a combination of development, security, and operations practices. It is a philosophy that aims to integrate security into the development process, rather than treating it as a separate step. This involves collaboration between development, security, and operations teams throughout the entire software development lifecycle (SDLC).

Some key differences between cybersecurity and DevSecOps include:

**Focus**: Cybersecurity is primarily focused on protecting systems from external threats, while DevSecOps focuses on integrating security into the development process.

**Scope**: Cybersecurity covers a wider range of topics, including network security, data security, application security, and more. DevSecOps, on the other hand, is specifically focused on improving the security of software development and deployment.

**Approach**: Cybersecurity typically involves implementing security measures after the development process is complete, while DevSecOps involves integrating security into the development process from the start.

**Collaboration**: Cybersecurity often involves collaboration between IT and security teams, while DevSecOps involves collaboration between development, security, and operations teams.

## Resources 

Over the course of the 90 Days, we will have a daily resources list that will bring relevant content that will help continue the topics and where you can go to find out more. 

- [TechWorld with Nana - What is DevSecOps? DevSecOps explained in 8 Mins](https://www.youtube.com/watch?v=nrhxNNH5lt0&list=PLsKoqAvws1pvg7qL7u28_OWfXwqkI3dQ1&index=1&t=19s)

- [What is DevSecOps?](https://www.youtube.com/watch?v=J73MELGF6u0&list=PLsKoqAvws1pvg7qL7u28_OWfXwqkI3dQ1&index=2&t=1s)

- [freeCodeCamp.org - Web App Vulnerabilities - DevSecOps Course for Beginners](https://www.youtube.com/watch?v=F5KJVuii0Yw&list=PLsKoqAvws1pvg7qL7u28_OWfXwqkI3dQ1&index=3&t=67s)

- [The Importance of DevSecOps and 5 Steps to Doing it Properly (DevSecOps EXPLAINED)](https://www.youtube.com/watch?v=KaoPQLyWq_g&list=PLsKoqAvws1pvg7qL7u28_OWfXwqkI3dQ1&index=4&t=13s)

- [Continuous Delivery - What is DevSecOps?](https://www.youtube.com/watch?v=NdvMUcWNlFw&list=PLsKoqAvws1pvg7qL7u28_OWfXwqkI3dQ1&index=5&t=6s)

- [Cloud Advocate - What is DevSecOps?](https://www.youtube.com/watch?v=a2y4Oj5wrZg&list=PLsKoqAvws1pvg7qL7u28_OWfXwqkI3dQ1&index=6)

- [Cloud Advocate - DevSecOps Pipeline CI Process - Real world example!](https://www.youtube.com/watch?v=ipe08lFQZU8&list=PLsKoqAvws1pvg7qL7u28_OWfXwqkI3dQ1&index=7&t=204s)

Hopefully this gave you a taster for what you can expect for this module and some of the resources above will help provide more depth on the topic, In the post on [Day 3](day03.md) we will be taking a look at what an attacker thinks like which is why we have to protect from the start.