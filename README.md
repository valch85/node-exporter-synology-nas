# node-exporter-synology-nas
Node-exporter & Prometeus in docker-compose for Synology NAS that send metrics to Grafana Cloud https://grafana.com

Use:
1. Clone repo
2. Add URL (from Grafan Cloud -> username -> Remote Write Endpoint)
3. Add username (from Grafan Cloud -> username -> Username / Instance ID)
4. Add password (from Grafan Cloud -> API Keys -> Add API Key)
5. Run `docker-compose up -d`
6. Go to Grafan Cloud
7. Verify that metrics are being ingested
  ![Alt text](<CleanShot 2024-01-20 at 02.43.35@2x.png>)
  ![Alt text](<CleanShot 2024-01-20 at 02.44.21@2x.png>)
8. If metrics are not present add rules to NAS firewall (taht will give permissoin resolve domain name inside of the container)
   ![Alt text](<CleanShot 2024-01-20 at 13.07.54@2x.png>)
9.  Add dashboard -> Import -> 1860 -> Load


