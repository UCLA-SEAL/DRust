# DRust
Language-Guided Distributed Shared Memory with Fine Granularity, Full Transparency, and Ultra Efficiency ([OSDI 2024](https://www.usenix.org/conference/osdi24/presentation/ma-haoran))

## Summary

Despite being a powerful concept, distributed shared memory (DSM) has not been made practical due to the extensive synchronization needed between servers to implement memory coherence. This project shows a practical DSM implementation based on the insight that the ownership model embedded in programming languages such as Rust automatically constrains the order of read and write, providing opportunities for significantly simplifying the coherence implementation if the ownership semantics can be exposed to and leveraged by the runtime. This project contains the design and implementation of DRust, a Rust-based DSM system that outperforms the two state-of-the-art DSM systems GAM and Grappa by up to 2.64× and 29.16× in throughput, and scales much better with the number of servers.

## Team
This project is done in collaboration with Professor [Harry Xu](http://web.cs.ucla.edu/~harryxu/)'s group at UCLA. Please visit [DRust project at UCLA Systems](https://github.com/uclasystem/drust). If you encounter any problems, please open an issue or feel free to contact us:

[Haoran Ma](https://www.haoranma.info/): [haoranma@ucla.edu](mailto:haoranma@ucla.edu).

## How to cite 
Please refer to our OSDI'24 paper, **[DRust: Language-Guided Distributed Shared Memory with Fine Granularity, Full Transparency, and Ultra Efficiency](https://www.usenix.org/conference/osdi24/presentation/ma-haoran)** for more details.

### Bibtex  
```txt
@inproceedings {ma2024drust,
author = {Haoran Ma and Yifan Qiao and Shi Liu and Shan Yu and Yuanjiang Ni and Qingda Lu and Jiesheng Wu and Yiying Zhang and Miryung Kim and Harry Xu},
title = {{DRust}: {Language-Guided} Distributed Shared Memory with Fine Granularity, Full Transparency, and Ultra Efficiency},
booktitle = {18th USENIX Symposium on Operating Systems Design and Implementation (OSDI 24)},
year = {2024},
isbn = {978-1-939133-40-3},
address = {Santa Clara, CA},
pages = {97--115},
url = {https://www.usenix.org/conference/osdi24/presentation/ma-haoran},
publisher = {USENIX Association},
month = jul
}
```
