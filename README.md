# playsc2
Try [pysc2](https://github.com/deepmind/pysc2) and update tutorial code.
來玩玩 pysc2，然後發現tutorial有點舊，所以來練習順便更新tutorial的code吧
## Run an default agent
```
python -m pysc2.bin.agent --map Simple64
```
## Run your own agent
```
python -m pysc2.bin.agent --map Simple64 --agent <path/to/agent>
```
## Play with agent
First, host the game with human interface on one terminal.
```
python -m pysc2.bin.play_vs_agent --human --map Simple64 --remote <port>
```
Second, run an agent to join the game using generated network config on another terminal.
Something like that.
```
python -m pysc2.bin.play_vs_agent --host 127.0.0.1 --config_port <the port displayed on host terminal>
```
