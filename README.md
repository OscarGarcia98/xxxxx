# xxxxx

            var alumno = new List<Alumno>();
            var agregar = true;

            while (agregar)
            {
                try
                {
                    bool result;
                    int mat = 0;
                    int aa = 0;
                    var a = new Alumno();
                    Console.WriteLine("Ingrese la matricula del alumno");
                    result = int.TryParse(Console.ReadLine(), out mat);
                    if (result == false)
                    {
                        Console.WriteLine("Ingrese un valor numerico");
                        
                    }
                    Console.WriteLine("Ingrese el nombre");
                    a.Nombre = Console.ReadLine();
                    Console.WriteLine("Ingrese la carrera del alumno");
                    a.Carrera = Console.ReadLine();
                    Console.WriteLine("Ingrese el semestre que está cursando");
                    a.Semestre = int.TryParse(Console.ReadLine(), out aa);
                    alumno.Add(a);
                    Console.WriteLine("Quiere agregar otro alumno: Y/N");
                   
                }
                catch 
                {
                    Console.WriteLine("Intente nuevamente");
                }
                if (Console.ReadLine() == "N")
                {
                    agregar = false;
                }
            }

            

            //Agregar conclusion apartir de las excepciones
