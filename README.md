<div align="center">

# Ren-Hao Deng

**M.S. in Computer Science @ National Taiwan University** · B.S. in CS @ NYCU

Systems software · LLM serving & inference systems · Computer vision · Backend infrastructure

[Email](mailto:ddeng691@gmail.com) · [LinkedIn](https://www.linkedin.com/in/dengrenhao)

</div>

---

## About

- Industry experience at **Trend Micro**, the **Institute for Information Industry (III)**, and **Academia Sinica**: evaluation frameworks for LLM-agent tool interfaces, LLM training pipelines on DGX clusters (DeepSpeed/LoRA), multi-agent LLM systems, and edge AI deployment in C++.
- **Computer vision** from classical operators to deployed systems: object detection and multi-object tracking, domain adaptation for cross-domain species classification, and a real-time tracking pipeline served as low-latency HLS.
- Comfortable across the stack, from **CUDA kernels, MPI/AVX-512 optimization, and SSD firmware simulation** to **concurrent network servers and containerized Linux infrastructure**.

> Most of my recent work (internships, thesis research) lives in private repositories; the projects below are a curated public subset.

## Research & Publications

- **EvolVE: Evolutionary Search for LLM-based Verilog Generation and Optimization**
  Hsin, W.\*, **Deng, R.**\*, Hsieh, Y.\*, Huang, E. & Hung, S. · *arXiv:2601.18067*, 2026. (\*equal contribution) [[paper]](https://arxiv.org/abs/2601.18067)
- **Structured Testbench Generation for LLM-Driven HDL Design and Verification-Oriented Data Curation**
  Huang, E., Kao, Y., **Deng, R.**, et al. · *arXiv:2606.12983*, 2026. [[paper]](https://arxiv.org/abs/2606.12983)
- **Exploring relationships among soundscape perception, spatiotemporal sound characteristics, and personal traits through social media**
  Chan, T., Wu, B., Lee, Y., Lee, P. & **Deng, R.** · *Noise Mapping*, 10(1), 2023. [[paper]](https://doi.org/10.1515/noise-2022-0174)

## Selected Projects

### Systems & Parallel Computing

| Project | Description | Tech |
|---|---|---|
| [hpc-kernel-optimization](https://github.com/dengrenhao/hpc-kernel-optimization) | Step-by-step kernel optimization: attention kernel from 241s to 3.2s (75.6×) on a 4-node cluster | C, CUDA, OpenMP, MPI, AVX-512 |
| [p-language-compiler](https://github.com/dengrenhao/p-language-compiler) | Full compiler for the P language: scanner → parser → AST → semantic analysis → RISC-V codegen | C/C++, flex, bison, RISC-V |
| [ssd-ftl-labs](https://github.com/dengrenhao/ssd-ftl-labs) | Instrumenting SSD internals in the MQSim simulator: FTL mapping-table hit rate, GC, and wear leveling (incl. an upstream bug fix) | C++, Python |
| [unix-systems-programming](https://github.com/dengrenhao/unix-systems-programming) | A ptrace + Capstone instruction-level debugger, and an LD_PRELOAD syscall-interception sandbox | C/C++, ptrace |
| [mips-cpu-verilog](https://github.com/dengrenhao/mips-cpu-verilog) | MIPS processor built bottom-up in Verilog: structural ALU, single-cycle datapath, and 5-stage pipeline | Verilog |
| [verilog-handwritten-digit-recognition](https://github.com/dengrenhao/verilog-handwritten-digit-recognition) | MNIST neural-network inference implemented entirely in Verilog (FSM-driven), with an interactive Python GUI | Verilog, Python |

### Backend & Infrastructure

| Project | Description | Tech |
|---|---|---|
| [network-programming](https://github.com/dengrenhao/network-programming) | Concurrent network servers from scratch: piped remote shell, multi-user server (select / fork + shared memory), HTTP+CGI, SOCKS4 proxy | C++, BSD sockets, boost.asio |
| [onos-virtual-router](https://github.com/dengrenhao/onos-virtual-router) | SDN virtual BGP router as an ONOS application: intent-based forwarding, Quagga peering, ARP gateway, DHCP relay | Java, ONOS, BGP, Mininet |
| [spark-bigdata-analytics](https://github.com/dengrenhao/spark-bigdata-analytics) | Big-data analytics on multi-million-row datasets with PySpark, Spark MLlib, and a self-provisioned GCP Dataproc cluster | PySpark, Hadoop, GCP |
| [freebsd-sysadmin-toolkit](https://github.com/dengrenhao/freebsd-sysadmin-toolkit) | FreeBSD sysadmin tools: a ZFS snapshot-backup CLI, an rc.d FTP upload-policy monitor, and a JSON container decoder | Shell, FreeBSD |
| [smart-fridge](https://github.com/dengrenhao/smart-fridge) | Multi-user smart fridge on Raspberry Pi: face recognition, Gemini-based item detection, per-user inventory via Telegram bot | Python, Raspberry Pi |

### Computer Vision

| Project | Description | Tech |
|---|---|---|
| [video-tracking-and-streaming](https://github.com/dengrenhao/video-tracking-and-streaming) | Classification → YOLOX detection with an SE-attention neck → ByteTrack MOT → a real-time tracker served to the browser as low-latency HLS at 30 FPS | PyTorch, OpenCV, ffmpeg, Flask |
| [uav-autopilot-vision](https://github.com/dengrenhao/uav-autopilot-vision) | Autonomous Tello flight from vision alone: camera calibration, ArUco pose + PID visual servoing, a fine-tuned YOLOv7-tiny detector, and grid-based line following | Python, OpenCV, PyTorch |
| [image-processing-and-colorization](https://github.com/dengrenhao/image-processing-and-colorization) | Histogram equalization/specification, Gaussian convolution, bicubic interpolation and Butterworth notch filtering implemented from the arithmetic up, applied to archival photo restoration | NumPy, OpenCV |

### Applied AI / ML

| Project | Description | Tech |
|---|---|---|
| [multimodal-lora-gapro](https://github.com/dengrenhao/multimodal-lora-gapro) | Combining LoRA-GA initialization with LoRA-Pro gradient correction on multimodal LLMs (LLaVA, Qwen-VL); unified training/eval framework with DeepSpeed | Python, PyTorch, DeepSpeed |
| [nlp-and-llm-finetuning](https://github.com/dengrenhao/nlp-and-llm-finetuning) | Four NLP tasks from BiLSTM-attention to LoRA fine-tuning of Vicuna-7B; using one LLM to filter another's context lifts accuracy 0.714 → 0.802 | Python, PyTorch, FastChat, LoRA |
| [ai-capstone](https://github.com/dengrenhao/ai-capstone) | Search, inference & ML agents: hand-written MCTS and a CNF-resolution Minesweeper solver | Python |
| [decision-tree-implementation](https://github.com/dengrenhao/decision-tree-implementation) | CART classification tree from scratch with linear-time incremental Gini split search | Python, NumPy |
| [Suika-Game-DRL-Final](https://github.com/dengrenhao/Suika-Game-DRL-Final) | Deep RL agents for the Suika game across four observation/action difficulty levels | Python, PyTorch |
| [AI_Project](https://github.com/dengrenhao/AI_Project) | Icon style transfer with CycleGAN and pix2pix implemented from the papers | Python, PyTorch |

### Research & Team Collaborations

- [EvolVE](https://github.com/evolution-lab-group/EvolVE): evolutionary search for LLM-based Verilog generation ([arXiv:2601.18067](https://arxiv.org/abs/2601.18067)); co-first author.
- [AnimeFrameBot](https://github.com/XYFC128/AnimeFrameBot): Go API server with fuzz/mutation testing; contributed the `/frame` and `/upload` API endpoints, fuzz tests and coverage, and the Telegram bot functions.
- [ICRTL-Benchmark](https://github.com/weiber2002/ICRTL-Benchmark): industrial-level RTL design challenges for evaluating LLM-based RTL generation; research collaboration (follow-up to EvolVE).



## Honors & Awards

| Award | Detail |
|---|---|
| **Global Winner**, NASA International Space Apps Challenge (2022) | Global Connection Award, Top 10 of 5,327 teams · [3D_ISS_Tracker](https://github.com/dengrenhao/3D_ISS_Tracker) |
| **Team of Excellence (Top 5)**, Taiwan Presidential Hackathon (2024) | "Quiet Tracker", edge-AI urban noise governance |
| **1st Place**, Data De-identification and Re-identification Competition, Academia Sinica (2023) | |
| **3rd Place**, Meichu Hackathon, NXP Enterprise Award (2023) | |
| **1st Place**, Meichu Hackathon, STMicroelectronics Enterprise Award (2022) | |

## Technical Skills

| Category | Technologies |
|---|---|
| Languages | C/C++, Python |
| Systems & Infrastructure | Linux (Arch/Ubuntu), Docker, Kubernetes, Ansible, PostgreSQL, Git/GitLab, GitHub Actions |
| Parallel & GPU Computing | CUDA, OpenMP, MPI, SIMD (AVX-512) |
| AI & GenAI | PyTorch, vLLM, SGLang, DeepSpeed, LangGraph, LLM fine-tuning (LoRA), RAG, multi-agent systems, MCP tools, LLM evaluation (LLM-as-judge) |

