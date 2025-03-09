            Film newestFilm = filmCollection[0];
            foreach (Film film in filmCollection)
            {
                if (film.year > newestFilm.year)
                {
                    newestFilm = film;
                }
            }
            Console.WriteLine($"The newest film is: {newestFilm.title}");


            for (int i = 0; i < filmCollection.Length; i++)
            {
                if (filmCollection[i].title == "Ant-Man")
                {
                    filmCollection[i] = new Film(filmCollection[i].title, filmCollection[i].certificate, filmCollection[i].year, true);
                }
            }

          
            foreach (Film film in filmCollection)
            {
                Console.WriteLine($"{film.title} - Being shown: {film.beingShown}");
            }
