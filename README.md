# ECOnodes.AI DeFi Optimizer

A full-stack web application that optimizes cross-chain DeFi transactions using Agentic AI with LangGraph orchestration. Built with Next.js and deployed on Vercel.

## 🚀 Features

- **Cross-Chain Transaction Optimization**: Find the most efficient routes across multiple blockchain networks
- **Agentic AI System**: Multi-agent orchestration with specialized Cost, Speed, and Carbon agents
- **Advanced Optimization Algorithms**: TOPSIS, Genetic Algorithm, Reinforcement Learning, and Pareto optimization
- **Real-Time Data Integration**: Live gas prices, network congestion, and carbon footprint tracking
- **RAG-Enhanced Decision Making**: Historical pattern analysis and market condition insights
- **Modern UI/UX**: Clean dashboard with interactive visualizations and real-time updates

## 🏗️ Architecture

### Frontend (Next.js + Tailwind)
- Clean, dashboard-style UI with responsive design
- Real-time transaction path visualization
- Comparison tables showing AI-optimal vs user-selected routes
- Interactive chain selection and optimization preferences

### Backend (Next.js API Routes)
- Web3 API integration (Alchemy, Infura, Covalent)
- Carbon footprint calculation using environmental APIs
- Mock/simulated transaction routing for demo purposes

### Agentic AI Layer (LangGraph Orchestration)
- **Cost Agent**: Evaluates transaction fees and finds cost-effective routes
- **Speed Agent**: Predicts latency and confirmation times
- **Carbon Agent**: Estimates energy usage and carbon footprint
- **Coordinator Agent**: Balances all factors and proposes optimal paths

### AI/ML Optimization
- **Reinforcement Learning**: Q-learning for route selection optimization
- **Heuristic Algorithms**: TOPSIS, Genetic Algorithm, Pareto frontier analysis
- **RAG System**: Retrieval-augmented generation for blockchain state analysis
- **Explainable AI**: Clear reasoning for route recommendations

## 🛠️ Installation

1. **Clone the repository**
   \`\`\`bash
   git clone <repository-url>
   cd econodes-ai-defi-optimizer
   \`\`\`

2. **Install dependencies**
   \`\`\`bash
   npm install
   \`\`\`

3. **Set up environment variables**
   \`\`\`bash
   cp .env.example .env.local
   \`\`\`
   Edit `.env.local` with your API keys:
   - Alchemy API key for Web3 data
   - Infura API key for blockchain access
   - Covalent API key for transaction data
   - Climatiq API key for carbon calculations

4. **Run the development server**
   \`\`\`bash
   npm run dev
   \`\`\`

5. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🚀 Deployment

### Vercel Deployment (Recommended)

1. **Connect to Vercel**
   \`\`\`bash
   npm i -g vercel
   vercel
   \`\`\`

2. **Set environment variables in Vercel dashboard**
   - Go to your project settings
   - Add all environment variables from `.env.example`
   - Deploy with `vercel --prod`

3. **Configure custom domain** (optional)
   - Add your domain in Vercel dashboard
   - Update DNS settings as instructed

### Manual Deployment

1. **Build the application**
   \`\`\`bash
   npm run build
   \`\`\`

2. **Start production server**
   \`\`\`bash
   npm start
   \`\`\`

## 🔧 Configuration

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `ALCHEMY_API_KEY` | Alchemy API key for Web3 data | Yes |
| `INFURA_API_KEY` | Infura API key for blockchain access | Yes |
| `COVALENT_API_KEY` | Covalent API key for transaction data | Yes |
| `CLIMATIQ_API_KEY` | Climatiq API key for carbon calculations | Yes |
| `ENABLE_REAL_TIME_DATA` | Enable live data fetching | No |
| `ENABLE_ADVANCED_OPTIMIZATION` | Enable advanced AI algorithms | No |
| `MAX_CONCURRENT_REQUESTS` | API rate limiting | No |

### Feature Flags

- **Real-Time Data**: Toggle live blockchain data vs mock data
- **Advanced Optimization**: Enable/disable complex algorithms
- **Carbon Tracking**: Toggle environmental impact calculations

## 📊 API Endpoints

### Core APIs
- `GET /api/chains?chainId={id}` - Get chain data and gas prices
- `POST /api/bridge-routes` - Find available bridge routes
- `POST /api/carbon-footprint` - Calculate carbon impact
- `POST /api/ai-optimize` - AI-powered route optimization
- `POST /api/optimize-advanced` - Advanced optimization algorithms

### Health & Monitoring
- `GET /api/health` - Application health check
- `GET /health` - Alias for health endpoint

## 🤖 AI Agents

### Cost Agent
- Analyzes transaction fees across different protocols
- Considers gas price volatility and network congestion
- Provides cost-efficiency scoring and savings calculations

### Speed Agent
- Predicts transaction confirmation times
- Factors in network congestion and block times
- Optimizes for fastest execution paths

### Carbon Agent
- Estimates energy consumption per blockchain
- Calculates carbon footprint for different routes
- Promotes eco-friendly transaction paths

### Coordinator Agent
- Orchestrates decisions from all specialized agents
- Applies user preferences and weighting
- Generates final recommendations with explanations

## 🧪 Optimization Algorithms

### TOPSIS (Technique for Order Preference by Similarity)
- Multi-criteria decision analysis
- Ranks routes based on distance to ideal solution

### Genetic Algorithm
- Evolutionary optimization approach
- Finds optimal solutions through selection and mutation

### Reinforcement Learning
- Q-learning for route selection
- Learns from historical transaction outcomes

### Pareto Optimization
- Identifies non-dominated solutions
- Balances trade-offs between cost, speed, and carbon

## 🔍 Monitoring & Analytics

- **Health Checks**: Automated system health monitoring
- **Performance Metrics**: Response times and success rates
- **Usage Analytics**: Transaction volume and user patterns
- **Error Tracking**: Comprehensive error logging and alerts

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For support and questions:
- Create an issue in the GitHub repository
- Contact the development team
- Check the documentation and FAQ

## 🙏 Acknowledgments

- Built with Next.js and Vercel
- UI components from shadcn/ui
- Web3 data from Alchemy and Infura
- Carbon calculations from Climatiq
- Icons from Lucide React
