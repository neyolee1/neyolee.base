REPO TEMPLATE 
mkdir ai-dev-agent
cd ai-dev-agent
git init
echo "# AI Dev Agent (Local)" > README.md
# create .gitignore 
cat <<EOL > .gitignore
.env
node_modules/
_pycache_/
*.log
EOL
# empty env (optional)
touch .env
touch http://agent.py
touch agent_prompt.txt
git add .
git commit -m "init: secure local setup"
SCRIPT
import os
import time
import random
from datetime import datetime
FILES = ["http://app.py", "http://utils.py", "data.txt"]
def ask_local_ai(prompt):
    return os.popen(f'ollama run llama3 "{prompt}"').read()
    def ensure_files():
    for f in FILES:
        if not os.path.exists(f):
            with open(f, "w") as file:
                file.write("# init\n")
                def apply_change(content):
    file = random.choice(FILES)
    with open(file, "a") as f:
        f.write(f"\n# update {http://datetime.now()}\n")
        f.write(content[:200])
        def commit(msg):
    os.system("git add .")
    os.system(f'git commit -m "{msg}"')
    def run():
    ensure_files()
    prompt = open("agent_prompt.txt").read()
    while True:
        output = ask_local_ai(prompt)
        apply_change(output)
        msg = "auto: " + output.split("\n")[0][:60]
        commit(msg)
        sleep = random.randint(60, 300)
        print(f"commit atıldı → bekleniyor {sleep}s")
        time.sleep(sleep)
        if neyolee
        == "_main_":
    run()# neyolee.base
