# Hi, I'm Inkiiee | 안녕하세요, 이인기입니다

**Embedded Linux · Network Systems · Robotics Software Engineer**

`C++` · `C` · `Linux` · `Yocto` · `Asio` · `OpenSSL` · `eBPF` · `ROS 2` · `Qt`

I build reliable C++ software at the boundary between devices and networks.<br>
장치와 네트워크의 경계에서 오래 안정적으로 동작하는 C++ 소프트웨어를 만듭니다.

My work focuses on embedded Linux networking and robotics, with failure recovery, bounded resource usage, concurrency, and observability treated as core design requirements.<br>
임베디드 Linux 네트워크 서비스와 로봇 소프트웨어를 주로 다루며, 정상 동작뿐 아니라 **장애 복구, 자원 상한, 동시성, 관측 가능성**까지 설계에 포함합니다.

## What I Work On | 주요 분야

- **Embedded Linux** — Yocto, ARMv8, resource-aware service design<br>
  제한된 CPU·메모리·저장 공간을 고려한 임베디드 서비스 설계
- **Async Networking** — C++20 coroutines, Asio channels, bounded queues, backpressure, timeouts
- **HTTP & TLS** — HTTP/1.1 framing, OpenSSL, certificate verification, connection lifecycle
- **Linux Data Path** — tc/eBPF, BPF maps, perf buffer, ring buffer 기반 이벤트 처리
- **Robotics** — ROS 2, LiDAR, SLAM, path planning, Qt visualization

## Featured Projects | 대표 프로젝트

### [Async Proxy](https://github.com/Inkiiee/asyn-proxy)

A resource-bounded HTTP/HTTPS reverse proxy built with C++20 coroutines, standalone Asio, and OpenSSL.<br>
C++20 코루틴 기반으로 구현한 **자원 제한형 HTTP/HTTPS 리버스 프록시**입니다.

- Concurrent HTTP/HTTPS listeners and HTTP/HTTPS upstream support
- Bounded sessions, queued jobs, and process-wide in-flight bytes
- Strict HTTP/1.1 framing validation, TLS verification, and explicit timeouts
- HTTP parser unit tests and plain HTTP/TLS integration tests

`C++20` `Coroutines` `Asio` `OpenSSL` `HTTP/1.1`

### [C++ 2D Navigation Stack](https://github.com/Inkiiee/cpp-2d-navigation-stack)

A ROS 2 autonomous navigation stack with custom 2D SLAM, global planning, and local obstacle avoidance.<br>
ROS 2 센서 파이프라인부터 지도 작성과 경로 주행까지 구성한 **2D 자율주행 실험 프로젝트**입니다.

- ICP, NDT, and CSM scan matching with occupancy grid mapping
- Submaps, loop closure, and pose graph optimization
- A* global planning, Pure Pursuit, and local obstacle handling
- Qt based mapping and navigation visualization

`C++` `ROS 2` `SLAM` `A*` `Pure Pursuit` `Qt 6`

### [Asio HTTP File Server](https://github.com/Inkiiee/asio-http-file-server)

An asynchronous HTTP file server and WebDAV experiment written in C++20.<br>
C++20과 standalone Asio로 구현한 **비동기 HTTP 파일 서버**입니다.

- File upload/download, byte range requests, and conditional requests
- JSON file management API and WebDAV methods
- URL handling and document-root traversal protection

`C++20` `Asio` `HTTP` `WebDAV`

### [Asio File Transfer Server](https://github.com/Inkiiee/asio-file-transfer-server)

An asynchronous file transfer server using TCP, UDP discovery, and a custom binary protocol.<br>
TCP 전송과 UDP 탐색을 결합한 **코루틴 기반 파일 전송 서버**입니다.

- Bounded asynchronous sessions and file transfer jobs
- TCP file transport with UDP service discovery
- Custom binary framing and connection lifecycle management

`C++20` `Coroutines` `Asio` `TCP` `UDP`

## Production Engineering | 실무 엔지니어링

Production source code and product-specific protocol details are private. The following lists only publicly shareable engineering experience.<br>
업무 프로젝트의 소스와 제품별 프로토콜은 비공개이며, 아래에는 공개 가능한 기술 경험만 정리합니다.

- Redesigned blocking network flows as coroutine-based relay pipelines with bounded queues
- Designed multi-endpoint failover and connection-state-based bypass control
- Integrated HMAC and AES-GCM protocols with explicit key lifecycle handling
- Added bounded streaming paths, disk reserve checks, and segmented log storage
- Measured RSS, anonymous memory, and file descriptors under repeated TLS connection load
- Diagnosed transaction, null-handling, key-processing, and DB concurrency failures from device logs and reproducible scenarios

## How I Work | 업무 방식

- I design failure and recovery paths together with the successful path.<br>
  정상 경로와 함께 **실패 상태와 복구 경로**를 설계합니다.
- I place explicit limits on queues, sessions, messages, and files.<br>
  큐, 세션, 메시지와 파일에 명시적인 상한을 둡니다.
- I narrow hypotheses with logs and measurements, then report reproducible conditions.<br>
  로그와 측정값으로 가설을 좁히고 재현 가능한 조건으로 문제를 전달합니다.
- I separate components by responsibility and lifetime while keeping shared logic in one place.<br>
  컴포넌트를 책임과 수명 주기로 분리하고 공통 로직은 한곳에서 관리합니다.

## Other Projects | 기타 프로젝트

- [Qt Packet Capture Lab](https://github.com/Inkiiee/qt-pcap-network-lab) — Qt/QML and libpcap based networking experiments
- [QML Tetris](https://github.com/Inkiiee/qml-tetris) — Tetris implemented with Qt/QML and C++
- [QML 2048](https://github.com/Inkiiee/qml-2048) — 2048 implemented with Qt/QML
- [SimpleFTP](https://github.com/Inkiiee/SimpleFTP) — FTP client with a Qt/QML interface

---

Public repositories contain personal study and portfolio work.<br>
공개 저장소에는 개인 학습 및 포트폴리오 프로젝트만 포함되어 있습니다.
