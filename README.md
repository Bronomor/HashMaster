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


###  Tytuł magisterki

Optymalizacja wyszukiwania podobnych obrazów w dużych bazach danych z wykorzystaniem specjalnych funkcji haszujących, uczenia maszynowego oraz technologii CUDA 

### wniosek

W ramach realizowanej pracy dyplomowej zostanie zaprojektowane oraz zaimplementowane rozwiązanie badające możliwość optymalizacji czasu wyszukiwania zdjęć w zbiorze ImageNet za pomocą zaadaptowania oraz dostosowania algorytmów LSH (Local Sensitive Hashing) oraz Neural Hashing z wykorzystaniem zrównoleglenia w technologii CUDA. Celem pracy jest stworzenie szybszej alternatywy do istniejących rozwiązań na CPU oraz GPU z wykorzystaniem uczenia maszynowego i technologii CUDA. W ramach pracy zostaną utworzone oraz zaimplementowane dwie specjalne funkcje haszujące, jedna klasyczna, ale zrównoleglona z wykorzystaniem API CUDA oraz druga z wykorzystaniem modeli uczenia maszynowego (bazująca na AI), też zaimplementowana z wykorzystaniem zrównoleglenia w technologii CUDA. Oba zaproponowane rozwiązania zostaną porównane z implementacjami funkcji haszujących dostępnych w bibliotekach – zarówno wykorzystujących do obliczeń CPU, jak i GPU. Proponowane w pracy rozwiązanie ma na celu rozwiązanie problemu wyszukiwania k-najbliższych sąsiadów, rozumianych jako zdjęcia identyczne lub podobne do danego na wejściu zdjęcia, z uniknięciem przeszukiwania całej bazy danych. Aby zrealizować ten cel koniecznym jest stworzenie struktury, która wstępnie pogrupuje zdjęcia ze zbioru ImageNet i skróci czas wyszukiwania podobnych zdjęć. Utworzenie tej struktury wymaga opracowania specjalnych algorytmów haszujących – algorytmy LSH oraz Neural Hashing, które umożliwią tworzenie podobnych haszy, dla podobnych obrazów, tworzenie tych haszy będzie między innymi w jednym z badanych rozwiązań odbywać się z wykorzystaniem sieci głębokich CNN (Convolutional Neural Network). Ostatecznym celem pracy jest zbadanie możliwości optymalizacji oraz przyśpieszenia wyszukiwania podobnych zdjęć w bardzo dużych bazach danych (testowy zbiór ImageNet ma około 14 mln zdjęć, testy będą realizowane na podzbiorze liczącym do 1 mln zdjęć) z wykorzystaniem technologii CUDA oraz specjalnych algorytmów (proponowane w pracy funkcje haszujące) oraz porównanie proponowanych rozwiązań z rozwiązaniami istniejącymi.
