This document contains an overview of Agentic AI frameworks (effective by Jul 2025).

## LangGraph
https://langchain-ai.github.io/langgraph/

LangGraph is an extension of LangChain (the same ecosystem). While it helps in some sense by being built on top of LangChain, the major difference in this framework is its paradigm in configuring the workflow. It is flexible on one hand, but as with great power comes great responsibility - it also becomes not trivial to keep configuring the workflow.
The workflows are being configured as a state machine - with edges pointing to where each state can transition from and to. If you feel comfortable with dealing with such precise configuration - LangGraph might be a good choice.

## Autogen (by Microsoft)
https://github.com/microsoft/autogen

## smolAgents
https://huggingface.co/docs/smolagents/en/index

## LLamaIndex
https://www.llamaindex.ai/

## Crew.AI
https://www.crewai.com/

Crew.ai is a great framework, very versatile, focused on how agents interact, how they solve the tasks, how they reason about problems. 
So basically it operates at a very higher level of concepts, rather than (comparing to other frameworks below) focusing on the lower level pluggable components that you can plug in knowing the pre-existing workflow or set of components you're planning to use.
Crew.ai is really good for making sure that a team (crew) of agents play together and work towards the goal of solving some task that they are supposed to.

What I really liked in Crew.AI is the configuration of agents so that you have to set the agent's role, goal and backstory. 
This structures behind the scenes the system prompts so well within the framework that you have to start thinking in terms of the higher level abstractions (the role, the goal, context, etc) rather that having to worry about drafting this all into the raw system prompt.

## Agno
https://www.agno.com/

Features:
1. ✔️ multitude of adapters for the possible LLM models and providers
2. ✔️ memory (extensible, but would love to get more plugins like Mem0 to be there)
3. ✔️ storage (session storage allowing use of SQLite, Mongo, Postgres, etc)
4. ✔️ knowledge (vector stores / RAG)
5. ✔️ tools (your custom tools, MCP, provided toolkits index)
6. ✔️ metrics collection extensible to OpenTelemetry based observability
7. ✔️ teams of agents
8. ✔️ user control flows

🌟 Agno is a real winner for me. Its a very well designed and maintained ecosystem with an extremely easy to use domain models of Agents and components. It also is extended with additional features, like the easy to bootstrap FastAPI application, playground application, UI (so good!) and even a basic eval framework.

## Other

### OpenAI Assistants
https://platform.openai.com/docs/assistants/overview

### BabyAGI
https://github.com/yoheinakajima/babyagi
Notable for being an experiment and a repo to "spark ideas and conversations". Honestly, this is still what is stays. Definitely don't intend using it for production purposes, mostly for inspiration and learning.
