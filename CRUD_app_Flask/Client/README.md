# React + Vite

# Project Setup Guide

Welcome to the project! This guide will walk you through setting up your development environment and ensuring you have the necessary dependencies installed on **Ubuntu**.

## Prerequisites

- **Node.js 21.x**
- **NPM** (Node Package Manager)

## Setup

Follow these steps to install and configure your development environment on **Ubuntu**:

### 1. Update and Upgrade Packages

Make sure your system is up to date.
 
# bash
sudo apt update
sudo apt upgrade

## Install Node.js 
-curl -fsSL https://deb.nodesource.com/setup_21.x | sudo -E bash -
-sudo apt install -y nodejs

## Verify Node.js installation:
-node -v

## Fix Missing Dependencies (if required)
-sudo apt-get install -f

## Check for Held Packages (Optional)-
**Sometimes packages are held back from upgrades. To check for such packages, use:--**
-sudo apt-mark showhold

## Install Project Dependencies-
-npm install
(This will install all required Node.js modules listed in the package.json file.)

## Verify NPM Version-
-npm -v


## Start Development Server-
-npm run dev





