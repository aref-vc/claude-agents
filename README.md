# Claude Code Custom Agents

A collection of specialized Claude Code subagents designed to enhance productivity across different business functions. These agents extend Claude Code's capabilities with domain-specific expertise and workflows.

## 🤖 What are Claude Code Agents?

Claude Code agents are specialized AI assistants that can be invoked using the `Task` tool within Claude Code. Each agent is designed with specific expertise, tools, and workflows to handle particular types of tasks more effectively than a general-purpose assistant.

## 📁 Agent Categories

### 🏢 Account Team Agents (5 agents)
Specialized agents for customer-facing roles and account management:

- **`account-executive-revenue-at`** - Strategic account management focused on revenue growth, retention analysis, and competitive positioning
- **`customer-success-manager-at`** - Analyze customer adoption patterns, assess value realization, and plan for renewals
- **`customer-support-at`** - Analyze support issues, track resolution patterns, and coordinate with product teams
- **`managed-services-engineer-at`** - Ensure product-customer alignment, manage release updates, and maintain implementation health
- **`product-engineer-at`** - Analyze customer use cases, map them to product capabilities, and identify feature gaps

### 📊 Market Research Agents (5 agents)
Agents specialized in market intelligence and competitive analysis:

- **`business-model-analyzer-mx`** - Research monetization strategies, analyze business models, and evaluate pricing approaches
- **`competitive-intelligence-mx`** - Comprehensive competitive analysis and market positioning insights
- **`experience-analyzer-mx`** - Analyze customer experience data to identify friction points and optimization opportunities
- **`reddit-intelligence-mx`** - Analyze Reddit communities for market intelligence, user sentiment, and trend identification
- **`tam-market-sizing-mx`** - Comprehensive market sizing analysis and total addressable market (TAM) calculations

### ⚡ Specialized Agents (4 agents)
General-purpose specialists for common business functions:

- **`content-marketer-writer`** - Create compelling, accessible content that explains complex topics to general audiences
- **`market-research-analyst`** - Comprehensive market intelligence and competitive analysis compiled into executive-ready reports
- **`product-requirements-generator`** - Create comprehensive Product Requirements Documents (PRDs) from initial ideas
- **`ui-ux-analyst`** - Expert UI/UX analysis, design feedback, and user experience optimization

## 🚀 How to Use

### Installation
1. Copy the desired agent `.md` files to your Claude Code agents directory:
   ```bash
   cp path/to/agent.md ~/.claude/agents/
   ```

2. Restart Claude Code or reload your configuration

### Usage Examples

```bash
# Use the product engineer agent to analyze a customer request
Task(
  description="Analyze customer integration needs",
  prompt="We have a customer who wants to integrate our API with their existing CRM system and needs real-time data sync capabilities",
  subagent_type="product-engineer-at"
)

# Use the market research agent for competitive analysis
Task(
  description="Research competitor pricing",
  prompt="Analyze pricing strategies for project management SaaS tools in the SMB market",
  subagent_type="business-model-analyzer-mx"
)

# Use the UX analyst for design feedback
Task(
  description="Review dashboard design",
  prompt="I've created a new analytics dashboard. Can you review the layout and suggest improvements?",
  subagent_type="ui-ux-analyst"
)
```

## 💡 Use Cases

### For Product Teams
- **Feature Planning**: Use `product-engineer-at` to map customer needs to product capabilities
- **Requirements Documentation**: Use `product-requirements-generator` to create comprehensive PRDs
- **UX Optimization**: Use `ui-ux-analyst` for design reviews and user experience improvements

### For Sales & Marketing
- **Account Management**: Use `account-executive-revenue-at` for strategic account planning
- **Content Creation**: Use `content-marketer-writer` for marketing materials and documentation
- **Market Research**: Use market research agents for competitive intelligence and sizing

### For Customer Success
- **Customer Health**: Use `customer-success-manager-at` to analyze adoption and retention
- **Support Optimization**: Use `customer-support-at` to identify and resolve systemic issues
- **Implementation Management**: Use `managed-services-engineer-at` for technical account management

### For Business Strategy
- **Market Analysis**: Use `tam-market-sizing-mx` for market opportunity assessment
- **Competitive Intelligence**: Use `competitive-intelligence-mx` for strategic positioning
- **Business Model Research**: Use `business-model-analyzer-mx` for monetization strategies

## 🔧 Customization

Each agent can be customized by modifying their `.md` files. Key areas to customize:

1. **Prompt Instructions**: Modify the core behavior and expertise areas
2. **Tool Access**: Specify which tools the agent should have access to
3. **Output Format**: Define how the agent should structure its responses
4. **Domain Knowledge**: Add specific industry or company context

## 📋 Requirements

- Claude Code CLI installed and configured
- Access to Claude Code's Task tool and subagent system
- Appropriate permissions for the tools each agent uses

## 🤝 Contributing

We welcome contributions! If you create useful agents or improvements:

1. Fork this repository
2. Add your agent with clear documentation
3. Include example use cases
4. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

These agents were developed to extend Claude Code's capabilities for common business workflows. They demonstrate the power of specialized AI agents for domain-specific tasks.

---

**Note**: These agents are extensions of Claude Code and require the Claude Code CLI to function. They are not standalone applications.