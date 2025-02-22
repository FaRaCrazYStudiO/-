# -
Менеджер через который можно будит запустить Ютуб, VPN? steam, telegram, VK, Yandex, discord, call of war, и всякие ссылки с ником meow*

import tkinter as tk
import webview
class WindowRuApp:
    def __init__(self, master):
        self.master = master
        self.master.title("WindowRuApp")
        self.master.geometry("800x600")
        
        self.btn_open_youtube = tk.Button(self.master, text="Открыть YouTube", command=self.open_youtube)
        self.btn_open_youtube.pack(pady=20)

        self.btn_open_steam = tk.Button(self.master, text="Открыть Steam", command=self.open_steam)
        self.btn_open_steam.pack(pady=10)

        self.btn_open_call_of_war = tk.Button(self.master, text="Открыть Call of war", command=self.open_call_of_war)
        self.btn_open_call_of_war.pack(pady=0)

        self.btn_open_vk = tk.Button(self.master, text="Открыть VK", command=self.open_vk)
        self.btn_open_vk.pack(pady=0)

        self.btn_open_yandex = tk.Button(self.master, text="Открыть Яндекс", command=self.open_yandex)
        self.btn_open_yandex.pack(pady=0)

        self.btn_open_discord = tk.Button(self.master, text="Открыть Discord", command=self.open_discord)
        self.btn_open_discord.pack(pady=0)
        
        self.btn_open_VPN = tk.Button(self.master, text="Запустить VPN", command=self.open_VPN)
        self.btn_open_VPN.pack(pady=0)

        self.btn_open_meow = tk.Button(self.master, text="meow", command=self.open_discord_link)
        self.btn_open_meow.pack(pady=0)

        self.btn_open_meow1 = tk.Button(self.master, text="meow1", command=self.open_author_link)
        self.btn_open_meow1.pack(pady=0)

        self.btn_open_meow2 = tk.Button(self.master, text="meow2", command=self.open_author_link1)
        self.btn_open_meow2.pack(pady=0)

        self.btn_open_tg = tk.Button(self.master, text="telegram", command=self.open_tg)
        self.btn_open_tg.pack(pady=0)


    def open_VPN(self):
        webview.create_window('VPN', 'https://t.me/NEODONbot?start=st', width=800, height=600)
        webview.start()
    def open_youtube(self):
        webview.create_window('YouTube', 'https://www.youtube.com', width=800, height=600)
        webview.start()

    def open_steam(self):
        webview.create_window('Steam', 'https://store.steampowered.com/join/completesignup', width=800, height=600)
        webview.start()

    def open_call_of_war(self):
        webview.create_window('Call of war', 'https://www.callofwar.com/', width=800, height=600)
        webview.start()

    def open_vk(self):
        webview.create_window('VK', 'https://vk.com/', width=800, height=600)
        webview.start()

    def open_yandex(self):
        webview.create_window('Яндекс', 'https://www.gs4u.net/ru/s/362340.html', width=800, height=600)
        webview.start()

    def open_discord(self):
        webview.create_window('Discord', 'https://discord.com/', width=800, height=600)
        webview.start()


    def open_discord_link(self):
        webview.create_window('meow', 'https://discord.gg/NCVT4CyUgu', width=800, height=600)
        webview.start()

    def open_author_link(self):
        webview.create_window('meowhiks', 'https://t.me/serverforkittens', width=800, height=600)
        webview.start()

    def open_author_link1(self):
        webview.create_window('meowhiks', 'https://t.me/meowka_a_ui', width=800, height=600)
        webview.start()

    def open_tg(self):
        webview.create_window('telegram', 'https://telegram.org/apps?ysclid=m7ghn4p0fw482294455', width=800, height=600)
        webview.start()


if __name__ == "__main__":
    root = tk.Tk()
    app = WindowRuApp(root)
    root.mainloop()
