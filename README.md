# 安装
    apt install ./v2raya.deb
# 下载
    https://release-assets.githubusercontent.com/github-production-release-asset/199570071/ecc6d661-3441-4216-bbd6-b65ba74ed5c2?sp=r&sv=2018-11-09&sr=b&spr=https&se=2026-11-17T04%3A17%3A05Z&rscd=attachment%3B+filename%3Dv2rayN-linux-64.deb&rsct=application%2Foctet-stream&skoid=96c2d410-5711-43a1-aedd-ab1947aa7ab0&sktid=398a6654-997b-47e9-b12b-9515b896b4de&skt=2026-11-17T03%3A16%3A16Z&ske=2026-11-17T04%3A17%3A05Z&sks=b&skv=2018-11-09&sig=kUXMDe2kgRXFdOM359RyrTXk3MSUrghBSaX%2Bfq5IFXc%3D&jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmVsZWFzZS1hc3NldHMuZ2l0aHVidXNlcmNvbnRlbnQuY29tIiwia2V5Ijoia2V5MSIsImV4cCI6MTc5NDg4NzMwNSwibmJmIjoxNzk0ODg1NTA1LCJwYXRoIjoicmVsZWFzZWFzc2V0cHJvZHVjdGlvbi5ibG9iLmNvcmUud2luZG93cy5uZXQifQ.BVo8PjKjs_M_OO8bMxHhI_xSNVhr0VKoNAySYSvkE_k&response-content-disposition=attachment%3B%20filename%3Dv2rayN-linux-64.deb&response-content-type=application%2Foctet-stream

# 设置开机自动启动
    systemctl enable v2raya.service

# 启动 v2rayA
    systemctl start v2raya.service

# 透明代理
    大陆白名单 (开启ip转发)

# 透明代理
    tproxy

# ----------------------

# mihomo
    chmod +x install_mihomo.sh && ./install_mihomo.sh

# 重载设置
    systemctl restart mihomo


