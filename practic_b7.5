

import random

#класс Корябля
class Ship:

    def __init__(self, name):
        self.name = name  
        self.damaged = False    

    #установим корабли на доске
    def Set_ships(self, Ships = [], bot = False):   

        Place_Ship_3 = False
        Place_Ship_2 = False
        Place_Ship_1 = False

        if len(Ships) > 0:
                
            _count = 0
               
            for i_ship_coords in Ships:
                 
                _count = 0

                if len(i_ship_coords) == 3:
                    Place_Ship_3 = True
                elif len(i_ship_coords) == 2:
                    Place_Ship_2 = True
                else:
                    Place_Ship_1 = True

                for j_ship_coords in i_ship_coords:
                    
                    try:
                        x = int(j_ship_coords[0])
                        y = int(j_ship_coords[1])
                    except ValueError:
                        print('Нужно вводить только целые числа!')

                    if self.check_ship(x, y, bot):
                        
                        _count += 1
                        
                        self.field[x-1][y-1] = '■'
                        self.NotAvailableCoords[x-1][y-1] = '■'

                        if Place_Ship_3:
                            self.Ship_3.append([x-1, y-1])
                            if _count == 3:
                                Place_Ship_3 = False
                                self.ban_coords(self.Ship_3)
                        elif Place_Ship_2:   
                            self.Ship_2.append([x-1, y-1])
                            if _count == 2:
                                Place_Ship_2 = False
                                self.ban_coords(self.Ship_2)    
                        else:
                            Place_Ship_1 = False
                            self.Ship_1.append([x-1, y-1])
                            self.ban_coords(self.Ship_1)
        
                    else:
                        pass

        else:

            Place_Ship_3 = True
            Place_Ship_2 = True
            Place_Ship_1 = True

            _count = 0
            
            #3 палубы
            while Place_Ship_3:

                ship_coords = input('Введите координаты корябля (3 палубы) : ').split()
                try:
                    x = int(ship_coords[0])
                    y = int(ship_coords[1])
                except ValueError:
                    print('Нужно вводить только целые числа!')

                if self.check_ship(x, y):
                    self.Ship_3.append([x-1, y-1])
                    self.field[x-1][y-1] = '■'
                    self.NotAvailableCoords[x-1][y-1] = '■'      
                    self.Print_Board()
                    _count += 1
                    if _count == 3:
                        Place_Ship_3 = False
                else:
                    self.Print_Board()
        
            _count = 0
            self.ban_coords(self.Ship_3)
            self.Print_Board()

            #2 палубы
            while Place_Ship_2:  

                ship_coords = input('Введите координаты корябля (2 палубы) : ').split()
                try:
                    x = int(ship_coords[0])
                    y = int(ship_coords[1])
                except ValueError:
                    print('Нужно вводить только целые числа!')

                if self.check_ship(x, y):
                    self.Ship_2.append([x-1, y-1])
                    self.field[x-1][y-1] = '■'
                    self.NotAvailableCoords[x-1][y-1] = '■'      
                    self.Print_Board()
                    _count += 1
                    if _count == 2:
                        self.ban_coords(self.Ship_2)
                        self.Print_Board()    
                    if _count == 4:
                        self.ban_coords(self.Ship_2)
                        Place_Ship_2 = False
                else:
                    self.Print_Board()

            _count = 0
            self.Print_Board()

            #1 палуба
            while Place_Ship_1: 

                ship_coords = input('Введите координаты корябля (1 палубы) : ').split()
                try:
                    x = int(ship_coords[0])
                    y = int(ship_coords[1])
                except ValueError:
                    print('Нужно вводить только целые числа!')

                if self.check_ship(x, y):
                    self.Ship_1.append([x-1, y-1])
                    self.field[x-1][y-1] = '■'
                    self.NotAvailableCoords[x-1][y-1] = '■'      
                    self.Print_Board()
                    _count += 1
                    if _count >= 1:
                        self.ban_coords(self.Ship_1)
                        self.Print_Board()
                    if _count == 4:
                        Place_Ship_1 = False
                else:
                    self.Print_Board()        

    #проверим доступность точек на доске
    def check_ship(self, x, y, bot = False):

        if bot:
            try:
                if x == 0 or y == 0 or x > 6 or y > 6:
                    raise IndexError
                if self.NotAvailableCoords[x-1][y-1] == 0 :
                    return True
                elif self.NotAvailableCoords[x-1][y-1] == '■':
                   #print(f"Поле {x},{y} уже занято")
                   return False
                else:
                    raise ValueError
            except ValueError:
                #print('Не правильные значения!!!!!')
                return False
            except IndexError:
                #print('Вышли за поля!!!!!!!!!')
                return False
        else:
            try:
                if x == 0 or y == 0 or x > 6 or y > 6:
                    raise IndexError
                if self.NotAvailableCoords[x-1][y-1] == 0 :
                    return True
                elif self.NotAvailableCoords[x-1][y-1] == '■':
                    print(f"Поле {x},{y} уже занято")
                else:
                    raise ValueError
            except ValueError:
                print('Не правильные значения!!!!!')
            except IndexError:
                print('Вышли за поля!!!!!!!!!')
                return False
        
    #заблокируем место на доске
    def ban_coords(self, Ship, shout_case = False):
                
        for i in Ship:
            x = i[0]
            y = i[1]
            if shout_case:
                try:
                    if x + 1 < 6:
                        if self.field[x+1][y] != '■':
                            self.NotAvailableCoords[x+1][y] = 'X'
                            self.field[x+1][y] = 'X'
                    if x + 1 < 6 and y - 1 >= 0:
                        if self.field[x+1][y-1] != '■':
                            self.NotAvailableCoords[x+1][y-1] = 'X'
                            self.field[x+1][y-1] = 'X'
                    if x + 1 < 6 and y + 1 < 6:
                        if self.field[x+1][y+1] != '■':
                            self.NotAvailableCoords[x+1][y+1] = 'X'
                            self.field[x+1][y+1] = 'X'
                    if x - 1 >= 0:
                        if self.field[x-1][y] != '■':
                            self.NotAvailableCoords[x-1][y] = 'X'
                            self.field[x-1][y] = 'X'
                    if x - 1 >= 0 and y - 1 >= 0:
                        if self.field[x-1][y-1] != '■':
                            self.NotAvailableCoords[x-1][y-1] = 'X'
                            self.field[x-1][y-1] = 'X'
                    if x - 1 >= 0 and y + 1 < 6:
                        if self.field[x-1][y+1] != '■':
                            self.NotAvailableCoords[x-1][y+1] = 'X'
                            self.field[x-1][y+1] = 'X'
                    if y + 1 < 6:
                        if self.field[x][y+1] != '■':
                            self.NotAvailableCoords[x][y+1] = 'X'
                            self.field[x][y+1] = 'X'
                    if y - 1 >= 0:
                        if self.field[x][y-1] != '■':
                            self.NotAvailableCoords[x][y-1] = 'X'  
                            self.field[x][y-1] = 'X'                                     
                except:
                    continue
            else:

                if self.field[x][y] == '■':
                    try:
                        if x + 1 < 6:
                            if self.field[x+1][y] != '■':
                                self.NotAvailableCoords[x+1][y] = 'X'
                        if x + 1 < 6 and y - 1 >= 0:
                            if self.field[x+1][y-1] != '■':
                                self.NotAvailableCoords[x+1][y-1] = 'X'
                        if x + 1 < 6 and y + 1 < 6:
                            if self.field[x+1][y+1] != '■':
                                self.NotAvailableCoords[x+1][y+1] = 'X'
                        if x - 1 >= 0:
                            if self.field[x-1][y] != '■':
                                self.NotAvailableCoords[x-1][y] = 'X'
                        if x - 1 >= 0 and y - 1 >= 0:
                            if self.field[x-1][y-1] != '■':
                                self.NotAvailableCoords[x-1][y-1] = 'X'
                        if x - 1 >= 0 and y + 1 < 6:
                            if self.field[x-1][y+1] != '■':
                                self.NotAvailableCoords[x-1][y+1] = 'X'
                        if y + 1 < 6:
                            if self.field[x][y+1] != '■':
                                self.NotAvailableCoords[x][y+1] = 'X'
                        if y - 1 >= 0:
                            if self.field[x][y-1] != '■':
                                self.NotAvailableCoords[x][y-1] = 'X'                                     
                    except:
                        continue

    def shout(self, AI_coords = []):
        
        self.damaged = False
        killed = False

        if self.name == 'Bot':
            print('---------------------------')
            shout_coords = input('Стреляю в : ' ).split()
            try:
                x = int(shout_coords[0])
                y = int(shout_coords[1])
            except ValueError:
                print('Нужно вводить только целые числа!')

            if self.field[x-1][y-1] == 'T':
                print('Опять в ту же точку... и опять мимо')
                self.damaged = True
                return 0

            if self.field[x-1][y-1] == '■':
                self.field[x-1][y-1] = 'X'
                self.Empty_field[x-1][y-1] = 'X'
                
                ship_3 = [x-1, y-1] in self.Ship_3
                ship_2 = [x-1, y-1] in self.Ship_2
                ship_1 = [x-1, y-1] in self.Ship_1

                if ship_3:
                    self.damaged = True
                    self.Ship_3.remove([x-1, y-1])
                    if len(self.Ship_3) == 0:
                        killed = True
                        print('Player убил!!!!!!!!!')
                    
                if ship_2:
                    self.damaged = True
                    self.Ship_2.remove([x-1, y-1])
                    if len(self.Ship_2) % 2 == 0:
                        killed = True
                        print('Player убил!!!!!!!!!')
                
                if ship_1:
                    self.damaged = True
                    self.Ship_1.remove([x-1, y-1])
                    killed = True
                    print('Player убил!!!!!!!!!')
            else:
                self.field[x-1][y-1] = 'T' 
                self.Empty_field[x-1][y-1] = 'T' 
                print('Player мимо')

            if self.damaged and not(killed):
                print('Player ранил')
                print('---------------------------') 
               
        else:

            if len(AI_coords) > 0:
                Ava_coords = AI_coords
            else:
                print('---------------------------')
                Ava_coords = self.Get_AvailableCoords(True)

            Coords_to_shout = random.choice(Ava_coords)
            x = Coords_to_shout[0]
            y = Coords_to_shout[1]
            #уберем этот выстрел из координатов бота
            Ava_coords.remove(Coords_to_shout)
            print(f'Bot стрельнул в {x}, {y}')
            print('---------------------------')
            if self.field[x-1][y-1] == '■':
                self.field[x-1][y-1] = 'X'
                
                ship_3 = [x-1, y-1] in self.Ship_3
                ship_2 = [x-1, y-1] in self.Ship_2
                ship_1 = [x-1, y-1] in self.Ship_1

                if ship_3:
                    self.damaged = True
                    self.Ship_3.remove([x-1, y-1])
                    if len(self.Ship_3) == 0:
                        killed = True
                        print('Bot убил!!!!!!!!!')
                    
                if ship_2:
                    self.damaged = True
                    self.Ship_2.remove([x-1, y-1])
                    if len(self.Ship_2) % 2 == 0:
                        killed = True
                        print('Bot убил!!!!!!!!!')
                
                if ship_1:
                    self.damaged = True
                    self.Ship_1.remove([x-1, y-1])
                    killed = True
                    print('Bot  убил!!!!!!!!!')
            else:
                self.field[x-1][y-1] = 'T'
                print('Bot мимо')
                
            
            if self.damaged and not(killed):
                print('Bot ранил')
                print('---------------------------') 
                AI_coords = [[x+1, y] if x + 1 < 6 else [], 
                             [x-1, y] if x - 1 > 0 else [], 
                             [x, y+1] if y + 1 < 6 else [], 
                             [x, y-1] if y - 1 > 0 else []]
                l_ = list(filter(None, AI_coords))
                self.shout(l_)
  
   
#класс Доски
class Board(Ship):
    
    def __init__(self, name):
        super().__init__(name)

    #сгенерируем доску
    def Create_Board(self):

        m = 6
        n = 6
        field = [[ i * 0 for j in range(m)] for i in range(n)]
        field_2 = [[ i * 0 for j in range(m)] for i in range(n)]
        self.field = field
        self.NotAvailableCoords = field_2
        self.Empty_field = [[ i * 0 for j in range(m)] for i in range(n)]

        self.Create_Ships()
        #self.Print_Board()
        #self.Set_ships()

    #создадим шаблон кораблей
    def Create_Ships(self):
        self.Ship_3 = []
        self.Ship_2 = []
        self.Ship_1 = []

    #сгенерируем корабли на доске
    def Generate_Bot_Ships(self, need_reboot = False):
        
        if need_reboot:
            return 0 
            
        list_ships = []

        #3 палубы
        coords_x = True if random.randint(0, 1) == 1 else False
       
        if coords_x:
            dot_x       = random.randint(1, 6)
            sec_dot_x   = random.choice([2, 2] if dot_x == 1 
                                        else [5, 5] if dot_x == 6
                                        else [dot_x - 1, dot_x + 1])
            third_dot_x = random.choice([3, 3] if dot_x == 1 or sec_dot_x == 1 
                                        else [4, 4] if dot_x == 6 or sec_dot_x == 6  
                                        else [sec_dot_x - 1, dot_x + 1] if sec_dot_x < dot_x
                                        else [dot_x - 1, sec_dot_x + 1])

            dot_y = sec_dot_y = third_dot_y = random.randint(1, 6)
        
        else:
            dot_y       = random.randint(1, 6)
            sec_dot_y   = random.choice([2, 2] if dot_y == 1 
                                        else [5, 5] if dot_y == 6
                                        else [dot_y - 1, dot_y + 1])
            third_dot_y = random.choice([3, 3] if dot_y == 1 or sec_dot_y == 1   
                                        else [4, 4] if dot_y == 6 or sec_dot_y == 6
                                        else [sec_dot_y - 1, dot_y + 1] if sec_dot_y < dot_y
                                        else [dot_y - 1, sec_dot_y + 1])

            dot_x = sec_dot_x = third_dot_x = random.randint(1, 6) 

        list_ships.append([
                            [dot_x, dot_y], 
                            [sec_dot_x, sec_dot_y], 
                            [third_dot_x, third_dot_y]
                        ])
        
        self.Set_ships(list_ships)
        #2 палубы
        list_ships = []

        while not(len(list_ships)) == 2:

            coords_x = True if random.randint(0, 1) == 1 else False
            
            if coords_x:
                dot_x       = random.randint(1, 6)
                sec_dot_x   = random.choice([2, 2] if dot_x == 1
                                            else [5, 5] if dot_x == 6 
                                            else [dot_x - 1, dot_x + 1])

                dot_y = sec_dot_y = random.randint(1, 6)
            
            else:
                dot_y       = random.randint(1, 6)
                sec_dot_y   = random.choice([2, 2] if dot_y == 1 
                                            else [5, 5] if dot_y == 6
                                            else [dot_y - 1, dot_y + 1])

                dot_x = sec_dot_x = random.randint(1, 6) 

            if self.check_ship(dot_x, dot_y, True) and self.check_ship(sec_dot_x, sec_dot_y, True):
               
                list_ships.append([
                            [dot_x, dot_y], 
                            [sec_dot_x, sec_dot_y]
                        ])
                

                self.Set_ships(list_ships, True)

        #self.Print_Board()
        #1 палуба
        list_ships = []

        while not(len(list_ships)) == 4:
            AvailableCoords = self.Get_AvailableCoords()
            if len(AvailableCoords) == 0:
                self.Create_Board()
                try:
                    self.Generate_Bot_Ships()
                    return 0 
                except RecursionError:
                    self.Generate_Bot_Ships(True)
                    return 0
                    

            else:
                dots = random.choice(AvailableCoords)  
                dot_x = dots[0]
                dot_y = dots[1]

                if self.check_ship(dot_x, dot_y, True):
                    
                    list_ships.append([
                                [dot_x, dot_y]
                            ])
                
                    self.Set_ships(list_ships, True) 
        
           
        #self.Print_Board()
        #self.Print_Not_Available()
        #для тестов
        # list_ships = [
        #             [[1, 2], [1, 3], [1, 4]], 
        #             [[3, 1], [3, 2]], 
        #             [[3, 4], [3, 5]],
        #             [[1, 6]], 
        #             [[5, 4]],
        #             [[6, 6]],
        #             [[6, 1]]
        #             ]
        # self.Set_ships(list_ships)
            
    def Get_AvailableCoords(self, field = False):
        
        AvailableCoords = []
        
        if field:
            for i in range(len(self.field)):
                    for j in range(len(self.field)):
                        if self.field[i][j] == 0 or self.field[i][j] == '■':
                            AvailableCoords.append([i+1, j+1])    
        else:
            for i in range(len(self.NotAvailableCoords)):
                for j in range(len(self.NotAvailableCoords)):
                    if self.NotAvailableCoords[i][j] == 0:
                        AvailableCoords.append([i+1, j+1])
            
        return AvailableCoords

    #выведем доску 
    def Print_Board(self):

        print('-----------BOT-------------') if self.name == 'Bot' else print('----------PLAYER-----------')

        coords = '  |', '1 |', '2 |', '3 |', '4 |', '5 |', '6 |'
        for i in coords:
            print(i, end = ' ')
        print()

        for i in range(len(self.field)):
            print(i+1, '|', end = ' ')
            for j in range(len(self.field)):
                print(self.field[i][j], '|', end = ' ')
            print()
        
    #пустая доска
    def Print_Empty_field(self):
        
        print('-----------BOT-------------') if self.name == 'Bot' else print('----------PLAYER-----------')

        coords = '  |', '1 |', '2 |', '3 |', '4 |', '5 |', '6 |'
        for i in coords:
            print(i, end = ' ')
        print()

        for i in range(len(self.Empty_field)):
            print(i+1, '|', end = ' ')
            for j in range(len(self.Empty_field)):
                print(self.Empty_field[i][j], '|', end = ' ')
            print()

    def Print_Not_Available(self):
        
        coords = '  |', '1 |', '2 |', '3 |', '4 |', '5 |', '6 |'
        for i in coords:
            print(i, end = ' ')
        print()

        for i in range(len(self.NotAvailableCoords)):
            print(i+1, '|', end = ' ')
            for j in range(len(self.NotAvailableCoords)):
                print(self.NotAvailableCoords[i][j], '|', end = ' ')
            print()
        print('---------------------------')         


Game = True 
Player_Move = random.randint(0, 1)

Bot_board = Board('Bot')
Bot_board.Create_Board()
Bot_board.Generate_Bot_Ships()

Player_board = Board('Player')
Player_board.Create_Board()
#установить свои корабли вручную
#Player_board.Print_Board()
#Player_board.Set_ships()
#сгенерировать корабли
Player_board.Generate_Bot_Ships()

Bot_board.Print_Board() 
Player_board.Print_Board()

print('Игра началась!')
while Game:
    if Player_Move:
        #читер мод. видно все корабли бота
        #Bot_board.Print_Board()
        Bot_board.Print_Empty_field()
        Bot_board.shout()
        if Bot_board.damaged:
            Player_Move = True
        else:
            Player_Move = False

        if len(Bot_board.Ship_3) == 0 and len(Bot_board.Ship_2) == 0 and len(Bot_board.Ship_1) == 0:
            print('=========== We have our champion! you will become Hokage !!! ============')
            print('Player - win!!! gz')
            Game = False

    else:
        Player_board.Print_Board()
        Player_board.shout()
        if Player_board.damaged:
            Player_Move = False
        else:
            Player_Move = True

        if len(Player_board.Ship_3) == 0 and len(Player_board.Ship_2) == 0 and len(Player_board.Ship_1) == 0:
            print('Bot wins!')
            Game = False
