# Agent Delegation Pattern

## Overview
This document describes the agent delegation pattern used in this project for tasks that benefit from specialized expertise.

## When to Delegate

Tasks should be delegated to custom agents when:
- A specialized agent exists for the task domain (e.g., cloud infrastructure, specific languages)
- The task requires domain-specific knowledge or tools
- The agent can provide higher quality results than general-purpose tools

## Available Agents

Currently, no custom agents are configured for this project. When custom agents become available, they will be documented here.

### Cloud Agent
**Status:** Not configured  
**Purpose:** Would handle cloud deployment, infrastructure, and serverless function optimization  
**Use Cases:**
- Vercel deployment configuration
- Cloud resource optimization
- Serverless function setup
- CDN configuration

## Usage Pattern

When a custom agent is available:
1. Identify the task requirements
2. Check if a relevant custom agent exists
3. Delegate the entire task to the agent with clear instructions
4. Accept the agent's work as final without additional validation

## Current Implementation

This project is deployed on Vercel (cloud platform) with the following configuration:
- Deployment: Automatic via Git integration
- Build: Next.js static site generation
- Files: Configured in `vercel.json` and `next.config.mjs`

For cloud-related tasks, manual configuration is currently required. See:
- `VERCEL_DEPLOYMENT.md` for deployment guide
- `vercel.json` for Vercel-specific settings
- `next.config.mjs` for Next.js build configuration
