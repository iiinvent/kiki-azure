# Kiki - Azure

A LiveKit-based project for real-time communication and streaming.

## Description

Kiki is a modern real-time communication platform built on LiveKit and Azure infrastructure, designed to provide seamless voice to voice audio streaming capabilities.

## Features

- Real-time video and audio streaming
- Azure cloud integration
- Scalable architecture
- Cross-platform compatibility

## Getting Started

### Prerequisites

- Node.js
- LiveKit server
- Azure account

### Installation

1. Clone the repository

```bash
git clone https://github.com/yourusername/kiki-azure.git
cd kiki-azure
```

1. Install dependencies

```bash
pnpm install
```

1. Configure environment variables

```bash
cp .env.example .env.local
# Edit .env with your configuration
```

1. Load environment variables

```powershell
(Get-Content .env.local) | Where-Object {$_ -notmatch '^#' -and $_.Trim()} | ForEach-Object { $key, $value = $_.Split('=', 2); [Environment]::SetEnvironmentVariable($key.Trim(), $value.Trim(), 'Process') }
```

1. Start the agent

```bash
pnpm exec tsx src/multimodal_agent.ts start
```

## Usage

LiveKit Voice to Voice agent for Microsoft Azure: [https://livekit.io/](https://livekit.io/)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [LiveKit](https://livekit.io/)
- [Azure](https://azure.microsoft.com/)
