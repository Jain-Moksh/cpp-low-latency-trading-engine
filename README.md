# Low-Latency Trading Systems Framework

Developed and maintained by **Moksh Jain** (GitHub: [@Jain-Moksh](https://github.com/Jain-Moksh), Email: [mokshjaindev@gmail.com](mailto:mokshjaindev@gmail.com)).

## Overview

This is a high-performance, production-grade C++ framework for building ultra-low-latency trading systems, designed for quantitative finance and systems programming. The focus is on highly efficient, clean, and cache-friendly code.

## Key Features

- 🚀 Sub-microsecond latency processing (blazingly fast IMO)
- 🔬 Statistical arbitrage strategy
- 🧊 Lock-free concurrent data structures
- 📊 Market data simulation (though, only a simulation)
- 🔍 Detailed performance benchmarking (run them yourself =)!)

## Performance Highlights

### Benchmark Results (M2 Max, macOS Sequoia)

#### Order Book Operations
- **Add Order**: 
  - Mean Latency: 347.20 ns
  - 99.9th Percentile: 2,458 ns
- **Best Bid/Ask Lookup**: 
  - Mean Latency: 14.32 ns
- **Cancel Order**: 
  - Mean Latency: 327.69 ns

#### Lock-Free Queue
- **Push/Pop Operations**: 
  - Mean Latency: ~14.5 ns
  - Consistently under 42 ns at 99th percentile

## Technical Architecture

### Components
- **Market Data Handler**: Real-time market data processing
- **Strategy Engine**: Advanced signal generation
- **Execution Engine**: Rapid order execution simulation
- **Utility Modules**: 
  - Lock-free queues
  - Memory pooling
  - Precise timing mechanisms

### Key Technologies
- Modern C++20
- Zero-overhead abstractions
- Cache-line optimized data structures
- Statistical arbitrage modeling

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/Jain-Moksh/cpp-low-latency-trading-engine.git
cd cpp-low-latency-trading-engine
```

### Prerequisites
- CMake (3.20+)
- Modern C++ Compiler (GCC 10+/Clang 10+/MSVC 19.2+)

### Build Instructions
```bash
mkdir build && cd build
cmake -DCMAKE_BUILD_TYPE=Release ..
make
```

### Run Benchmarks
```bash
# From build directory
./benchmark/latency_benchmark
```

### Run Market Simulator
```bash
# From build directory
./examples/simulator
```

## Performance Philosophy

Each line of code is crafted to minimize computational overhead and maximize throughput. 

## Potential Applications

- Algorithmic Trading Platforms
- Market Making Systems
- Quantitative Research Infrastructure
- High-Performance Financial Simulations
- Anything where you think that speed is key

## Author

**Moksh Jain**
- GitHub: [@Jain-Moksh](https://github.com/Jain-Moksh)
- Email: [mokshjaindev@gmail.com](mailto:mokshjaindev@gmail.com)

## Contributions

Feel free to open issues or submit pull requests. If you find potential for optimization or have any feedback, please reach out!

## License

This project is open-source and shared in the spirit of open collaboration and learning. You are free to:
- Use the code in personal or commercial projects
- Modify and adapt the code
- Share and distribute the code

Please provide proper attribution to the author.


