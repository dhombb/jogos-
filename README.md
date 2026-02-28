import requests

url = "https://exemplo.com/arquivo-publico.zip"
r = requests.get(url)

with open("arquivo.zip", "wb") as f:
    f.write(r.content)

print("Download concluído")
