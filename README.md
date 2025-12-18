# GamemodeChecker

[English](#english) | [日本語](#japanese)

---
Download(ダウンロード): https://modrinth.com/plugin/gamemodecheck/
---

## English

### Overview

GamemodeChecker is a Minecraft Spigot plugin that allows server administrators and operators to check players' game modes. You can check a specific player's game mode or view all online players grouped by their game modes.

### Features

- **Check Individual Player**: Check a specific player's game mode using their Minecraft username
- **List All Players**: View all online players organized by game mode
- **Tab Completion**: Auto-complete player names when typing the command
- **Customizable Messages**: All messages can be customized through the config.yml file
- **Permission-Based**: Uses Bukkit permissions for access control

### Requirements

- **Minecraft Version**: 1.20.1 or compatible
- **Server Software**: Spigot or Paper
- **Java Version**: 17 or higher

### Installation

1. Download the latest `GamemodeChecker-1.0-shaded.jar` from the releases
2. Place the JAR file in your server's `plugins` folder
3. Restart your server or use `/reload` command
4. The plugin will automatically create a `config.yml` file in the `plugins/GamemodeChecker` folder

### Usage

#### Check a Player's Game Mode
```
/gamemodecheck <player_name>
```

Example:
```
/gamemodecheck Steve
```

#### List All Players by Game Mode
```
/gamemodecheck *
```

This will display all online players grouped by their game modes (SURVIVAL, CREATIVE, ADVENTURE, SPECTATOR).

### Commands

| Command | Description | Permission |
|---------|-------------|------------|
| `/gamemodecheck <MCID\|*>` | Check a player's game mode or list all players by game mode | `gamemodecheck.use` |

### Permissions

| Permission | Description | Default |
|-----------|-------------|---------|
| `gamemodecheck.use` | Allows use of the /gamemodecheck command | OP |

### Configuration

The plugin creates a `config.yml` file with customizable messages:

```yaml
messages:
  usage: "&eUsage: /gamemodecheck <MCID|*>"
  no-permission: "&cYou do not have permission to use this command."
  player-not-found: "&cPlayer {player} not found."
  player-mode: "&6Player {player}'s game mode: &a{mode}"
  list-header: "&6Game Modes:"
  mode-format: "&e{mode}: &a{players}"
```

You can customize these messages using Minecraft color codes (`&` prefix).

### Building from Source

1. Clone this repository
2. Make sure you have Maven installed
3. Run the following command:
   ```bash
   mvn clean package
   ```
4. The compiled JAR file will be in the `target` folder

### License

This project is open source. Feel free to use and modify it as needed.

### Author

koirdsuzu

---

## Japanese

### 概要

GamemodeCheckerは、サーバー管理者やオペレーターがプレイヤーのゲームモードを確認できるMinecraft Spigotプラグインです。特定のプレイヤーのゲームモードを確認したり、ゲームモード別にすべてのオンラインプレイヤーを表示したりできます。

### 機能

- **個別プレイヤー確認**: Minecraftユーザー名を使用して特定のプレイヤーのゲームモードを確認
- **全プレイヤー一覧**: ゲームモード別に整理されたすべてのオンラインプレイヤーを表示
- **タブ補完**: コマンド入力時にプレイヤー名を自動補完
- **カスタマイズ可能なメッセージ**: config.ymlファイルを通じてすべてのメッセージをカスタマイズ可能
- **権限ベース**: アクセス制御にBukkit権限を使用

### 要件

- **Minecraftバージョン**: 1.20.1以上または互換バージョン
- **サーバーソフトウェア**: SpigotまたはPaper
- **Javaバージョン**: 17以上

### インストール

1. リリースから最新の `GamemodeChecker-1.0-shaded.jar` をダウンロード
2. JARファイルをサーバーの `plugins` フォルダに配置
3. サーバーを再起動するか `/reload` コマンドを使用
4. プラグインは自動的に `plugins/GamemodeChecker` フォルダに `config.yml` ファイルを作成します

### 使用方法

#### プレイヤーのゲームモードを確認
```
/gamemodecheck <プレイヤー名>
```

例:
```
/gamemodecheck Steve
```

#### ゲームモード別に全プレイヤーを一覧表示
```
/gamemodecheck *
```

これにより、ゲームモード（SURVIVAL、CREATIVE、ADVENTURE、SPECTATOR）別にすべてのオンラインプレイヤーが表示されます。

### コマンド

| コマンド | 説明 | 権限 |
|---------|------|------|
| `/gamemodecheck <MCID\|*>` | プレイヤーのゲームモードを確認するか、ゲームモード別に全プレイヤーを一覧表示 | `gamemodecheck.use` |

### 権限

| 権限 | 説明 | デフォルト |
|------|------|-----------|
| `gamemodecheck.use` | /gamemodecheckコマンドの使用を許可 | OP |

### 設定

プラグインはカスタマイズ可能なメッセージを含む `config.yml` ファイルを作成します：

```yaml
messages:
  usage: "&eUsage: /gamemodecheck <MCID|*>"
  no-permission: "&cYou do not have permission to use this command."
  player-not-found: "&cPlayer {player} not found."
  player-mode: "&6Player {player}'s game mode: &a{mode}"
  list-header: "&6Game Modes:"
  mode-format: "&e{mode}: &a{players}"
```

Minecraftのカラーコード（`&` プレフィックス）を使用してこれらのメッセージをカスタマイズできます。

### ソースからビルド

1. このリポジトリをクローン
2. Mavenがインストールされていることを確認
3. 次のコマンドを実行：
   ```bash
   mvn clean package
   ```
4. コンパイルされたJARファイルは `target` フォルダにあります

### ライセンス

このプロジェクトはオープンソースです。必要に応じて自由に使用および変更してください。

### 作者

koirdsuzu


