# HashMaster

## Run Project

To run project use the following commands
```
cd docker
docker-compose -f compilation.yaml -p <name> up -d
docker exec -it <name> bash
```

Where you are inside a container you can run notebook
```
python3 -m notebook --allow-root
```

From the predefined steps you can choose
1. LSH
2. NeuralHashing
3. cuLSH
4. NeuralHashing + cuLSH
5. Benchmarks