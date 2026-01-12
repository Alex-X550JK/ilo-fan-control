<div align="center">
  <h1 align="center">iLO Fan Control Dashboard</h1>
  <h1 align="center"><a href="https://github.com/alexgeraldo">by alexgeraldo</a></h1>
  <img src="docs/preview.png" height="450">

  <p align="center">
    HP iLO Fan Control Dashboard is a responsive web interface for controlling and monitoring fan speeds on HP Gen8 servers with <a href="https://github.com/kendallgoto/ilo4_unlock">unlocked iLO 4 firmware</a>. It combines FastAPI, HTMX and Bootstrap to offer real-time telemetry, manual/auto fan modes, and a seamless experience across devices.
  </p>
  <small><p align="center">Built for homelab users who want silence, efficiency, and control — no full-stack overhead required.</p></small>

</div>

## Changes
- Added SSH port specification
- Set **Manual Mode** as default start
- Changed speed setting from set value to max % (allows server to ajust up to that %)
  changed command from **lock** to **max**

## 🐳 Use with Docker

If you already have a Docker environment deployed, its best to get the app running in seconds.

```bash
docker run -d --rm \
  -p 8000:8000 \
  -e ILO_HOST="ilo-ip-address" \
  -e ILO_PORT="ssh port Nº" \
  -e ILO_USER="ilo-user" \
  -e ILO_PASS="ilo-password" \
  asilvaws/ilo-fans:latest
```

Then open [http://localhost:8000](http://localhost:8000) in your browser.


## 🙏 Acknowledgments

- [kendallgoto/ilo4_unlock](https://github.com/kendallgoto/ilo4_unlock) – for the unlocked iLO 4 firmware that makes all of this possible  
- [alex3025/ilo-fans-controller](https://github.com/alex3025/ilo-fans-controller) – inspiration from the original PHP fan controller project  
- [FastAPI](https://fastapi.tiangolo.com/) – for the web framework powering the backend  
- [HTMX](https://htmx.org/) – for enabling dynamic frontend interactivity without needing a JS framework  
- [Bootstrap](https://getbootstrap.com/) – for the responsive UI  
- [Font Awesome](https://fontawesome.com/) – for icons used in the dashboard UI  
- [Python](https://www.python.org/) – because, well... everything  
- The **homelab community** – for sharing tools, ideas, and firmware patches 😄


## 📄 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---

**📬 Stay Updated**  
Follow **[@alexgeraldo](https://github.com/alexgeraldo)** on GitHub.

---
