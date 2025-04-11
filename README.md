networks:
  opensis_network:
    external: true


  and I created the network before docker compose up
9:11
docker network create opensis_network
9:11
I did run docker compose -f docker-compose.yml -f docker-compose-oncall.yml up -d


then on grafana dash when I added the plug, got the same error that. we had earlier but running this comannd curl -X POST 'http://admin:admin@localhost:3000/api/plugins/grafana-oncall-app/settings' -H "Content-Type: application/json" -d '{"enabled":true, "jsonData":{"stackId":5, "orgId":100, "onCallApiUrl":"http://engine:8080/", "grafanaUrl":"http://grafana:3000/"}}'  that error was cleared





  