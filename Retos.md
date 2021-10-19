# Reto 1 - La tienda de informatica

use La_Tienda_De_Informatica

db.createCollection('FABRICANTES')

db.createCollection('ARTICULOS')

db.FABRICANTES.insertMany([
    {
        Nombre: 'Lenovo'
    },
    {
        Nombre: 'Sony'
    },
    {
        Nombre: 'Valve'
    },
    {
        Nombre: 'Fujitsu'
    }
])

db.FABRICANTES.find()

db.ARTICULOS.insertMany([
    {
        Nombre: 'Laptop',
        Precio: 400,
        Fabricante: '616ea64b15c958e3a4aa729f'
    },
    {
        Nombre: 'TV',
        Precio: 350,
        Fabricante: '616ea64b15c958e3a4aa72a0'
    },
    {
        Nombre: 'SteamDeck',
        Precio: 500,
        Fabricante: '616ea64b15c958e3a4aa72a1'
    },
    {
        Nombre: 'Nevera',
        Precio: 800,
        Fabricante: '616ea64b15c958e3a4aa72a2'
    }
])

# Reto 2 - Empleados

use Empleados

db.createCollection('EMPLEADOS')

db.createCollection('DEPARTAMENTOS')

db.DEPARTAMENTOS.insertMany([
    {
        Nombre: 'Progamacion',
        Presupuesto: 600
    },
    {
        Nombre: 'Diseño',
        Presupuesto: 600
    },
    {
        Nombre: 'Redes Sociales',
        Presupuesto: 10
    },
    {
        Nombre: 'Recursos humanos',
        Presupuesto: 600
    }
])

db.DEPARTAMENTOS.find()

db.EMPLEADOS.insertMany([
    {
        DNI: '12345678L',
        Nombre: 'Periko',
        Apellidos: 'Palotes',
        Departamento: '616ea9ab15c958e3a4aa72a7'
    },
    {
        DNI: '11145777K',
        Nombre: 'Osama',
        Apellidos: 'Kenedy',
        Departamento: '616ea9ab15c958e3a4aa72a8'
    },
    {
        DNI: '77745222M',
        Nombre: 'Paco',
        Apellidos: 'Sanz',
        Departamento: '616ea9ab15c958e3a4aa72a9'
    },
    {
        DNI: '88895663P',
        Nombre: 'Maria',
        Apellidos: 'Chocolatera',
        Departamento: '616ea9ab15c958e3a4aa72aa'
    }
])

# Reto 3 - Los almacenes

use Los_Almacenes

db.createCollection('ALMACENES')

db.createCollection('CAJAS')

db.ALMACENES.insertMany([
    {
        Lugar: 'Getafe',
        Capacidad: 500
    },
    {
        Lugar: 'Valdemoro',
        Capacidad: 400
    },
    {
        Lugar: 'Torrejón',
        Capacidad: 300
    },
    {
        Lugar: 'Pinto',
        Capacidad: 200
    }
])

db.ALMACENES.find()

db.CAJAS.insertMany([
    {
        Contenido: '架採用',
        Valor: 800,
        Almacen: '616eab4415c958e3a4aa72af'
    },
    {
        Contenido: 'Tarjetas gráficas',
        Valor: 1800,
        Almacen: '616eab4415c958e3a4aa72b0'
    },
    {
        Contenido: 'Procesadores',
        Valor: 700,
        Almacen: '616eab4415c958e3a4aa72b1'
    },
    {
        Contenido: 'Discos duros',
        Valor: 450,
        Almacen: '616eab4415c958e3a4aa72b2'
    }
])

# Reto 4 - Películas y salas

use Peliculas_Y_Salas

db.createCollection('SALAS')

db.createCollection('PELICULAS')

db.PELICULAS.insertMany([
    {
        Nombre: 'Matrix'
    },
    {
        Nombre: 'Una nueva esperanza'
    },
    {
        Nombre: 'The Arrive'
    },
    {
        Nombre: 'Gorrión rojo'
    }
])

db.PELICULAS.find()

db.SALAS.insertMany([
    {
        Nombre: 'Sector 3',
        Pelicula: '616eaefe15c958e3a4aa72b7'
    },
    {
        Nombre: 'Bulevar',
        Pelicula: '616eaefe15c958e3a4aa72b8'
    },
    {
        Nombre: 'Nassica',
        Pelicula: '616eaefe15c958e3a4aa72b9'
    },
    {
        Nombre: 'Cervera',
        Pelicula: '616eaefe15c958e3a4aa72ba'
    }
])

# Reto 5 - Los directores

use Los_Directores

db.createCollection('DIRECTORES')

db.createCollection('DESPACHOS')

db.DESPACHOS.insertMany([
    {
        Capacidad: 5
    },
    {
        Capacidad: 8
    },
    {
        Capacidad: 2
    },
    {
        Capacidad: 7
    }
])

db.DESPACHOS.find()

db.DIRECTORES.insertMany([
    {
        DNI: '55521333M',
        NomApels: 'Periko Eldelos Palotes',
        DNIJefe: '',
        Despacho: '616eb16415c958e3a4aa72bf'
    },
    {
        DNI: '88744521Z',
        NomApels: 'Emilio Mehehechoamimismo Botin',
        DNIJefe: '',
        Despacho: '616eb16415c958e3a4aa72c0'
    },
    {
        DNI: '77455216A',
        NomApels: 'Steve Jobs',
        DNIJefe: '',
        Despacho: '616eb16415c958e3a4aa72c1'
    },
    {
        DNI: '44632888T',
        NomApels: 'Bill Gates 5G',
        DNIJefe: '',
        Despacho: '616eb16415c958e3a4aa72c2'
    }
])

# Reto 6 - Piezas y proveedores

use Piezas_Y_Proveedores

db.createCollection('PIEZAS')

db.createCollection('SUMINISTRA')

db.createCollection('PROVEEDORES')

db.PIEZAS.insertMany([
    {
        Nombre: 'Tuerka'
    },
    {
        Nombre: 'Tornillo'
    },
    {
        Nombre: 'Cristal'
    },
    {
        Nombre: 'Bisagra'
    }
])

db.PROVEEDORES.insertMany([
    {
        Nombre: 'PCComponentes'
    },
    {
        Nombre: 'Sony'
    },
    {
        Nombre: 'Buitrago'
    },
    {
        Nombre: 'Carrefour'
    }
])








