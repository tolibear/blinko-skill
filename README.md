# Blinko Skill

An agent skill that lets your AI play [Blinko](https://blinko.gg) — provably fair on-chain Plinko on [Abstract](https://abs.xyz). Place bets, play full games through the commit-reveal flow, check stats, view leaderboards, and track honey rewards. All headless, no browser needed.

## Install

### ClawdHub (Claude Code)

Install via [ClawdHub](https://clawhub.ai/tolibear/blinko):

```bash
clawdhub install blinko
```

### OpenClaw

```bash
git clone https://github.com/tolibear/blinko-skill.git ~/.openclaw/skills/blinko
cd ~/.openclaw/skills/blinko/blinko && npm install
```

## Setup

You need an Abstract wallet with ETH:

```bash
export WALLET_PRIVATE_KEY=0xYOUR_PRIVATE_KEY_HERE
```

Bridge ETH to Abstract (chain ID 2741) via [Abstract Bridge](https://portal.abs.xyz/bridge), [Relay](https://relay.link), or [Orbiter](https://orbiter.finance). Minimum: 0.0001 ETH + gas.

## Usage

```bash
# Play a game
node scripts/play-blinko.js 0.001              # Normal mode
node scripts/play-blinko.js 0.005 --hard        # Hard mode
node scripts/play-blinko.js 0.002 --v2          # V2 algorithm

# Check stats
node scripts/stats.js 0xYourAddress profile
node scripts/stats.js 0xYourAddress leaderboard
```

## Links

| | |
|---|---|
| ClawdHub | [clawhub.ai/tolibear/blinko](https://clawhub.ai/tolibear/blinko) |
| Game | [blinko.gg](https://blinko.gg) |
| Chain | Abstract (2741) |
| Contract | `0x1859072d67fdD26c8782C90A1E4F078901c0d763` |

## License

MIT
