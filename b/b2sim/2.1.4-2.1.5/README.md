# Comparing `tmp/b2sim-2.1.4.tar.gz` & `tmp/b2sim-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-2.1.4.tar", last modified: Fri Apr 12 03:42:27 2024, max compression
+gzip compressed data, was "b2sim-2.1.5.tar", last modified: Wed May 15 20:00:49 2024, max compression
```

## Comparing `b2sim-2.1.4.tar` & `b2sim-2.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 03:42:27.877411 b2sim-2.1.4/
--rw-rw-rw-   0        0        0    35823 2023-05-09 05:51:58.000000 b2sim-2.1.4/LICENSE
--rw-rw-rw-   0        0        0      123 2024-02-07 03:13:22.000000 b2sim-2.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      385 2024-04-12 03:42:27.877411 b2sim-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    18853 2024-02-22 04:54:10.000000 b2sim-2.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 03:42:27.843930 b2sim-2.1.4/b2sim/
--rw-rw-rw-   0        0        0        0 2024-02-05 03:29:23.000000 b2sim-2.1.4/b2sim/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 03:42:27.863821 b2sim-2.1.4/b2sim/analysis/
--rw-rw-rw-   0        0        0      108 2024-02-12 21:33:54.000000 b2sim-2.1.4/b2sim/analysis/__init__.py
--rw-rw-rw-   0        0        0    24288 2024-02-19 21:31:12.000000 b2sim-2.1.4/b2sim/analysis/ai.py
--rw-rw-rw-   0        0        0     4346 2024-02-21 01:49:15.000000 b2sim-2.1.4/b2sim/analysis/fitness.py
--rw-rw-rw-   0        0        0     5061 2024-02-12 21:30:11.000000 b2sim-2.1.4/b2sim/analysis/graphing.py
--rw-rw-rw-   0        0        0     5674 2024-02-07 01:42:59.000000 b2sim-2.1.4/b2sim/analysis/visualize.py
-drwxrwxrwx   0        0        0        0 2024-04-12 03:42:27.871341 b2sim-2.1.4/b2sim/engine/
--rw-rw-rw-   0        0        0      102 2024-02-04 07:54:08.000000 b2sim-2.1.4/b2sim/engine/__init__.py
--rw-rw-rw-   0        0        0    14197 2024-02-23 22:29:57.000000 b2sim-2.1.4/b2sim/engine/actions.py
--rw-rw-rw-   0        0        0     6611 2024-02-08 21:38:28.000000 b2sim-2.1.4/b2sim/engine/farms.py
--rw-rw-rw-   0        0        0     9918 2024-02-08 21:25:01.000000 b2sim-2.1.4/b2sim/engine/info.py
--rw-rw-rw-   0        0        0   110575 2024-03-17 04:23:44.000000 b2sim-2.1.4/b2sim/engine/main.py
--rw-rw-rw-   0        0        0     5069 2024-02-09 00:43:24.000000 b2sim-2.1.4/b2sim/engine/rounds.py
-drwxrwxrwx   0        0        0        0 2024-04-12 03:42:27.874341 b2sim-2.1.4/b2sim/templates/
--rw-rw-rw-   0        0        0     1944 2024-02-19 06:29:12.000000 b2sim-2.1.4/b2sim/templates/config.txt
--rw-rw-rw-   0        0        0     2027 2024-04-12 03:06:06.000000 b2sim-2.1.4/b2sim/templates/eco_send_info.csv
--rw-rw-rw-   0        0        0      613 2023-07-19 19:03:45.000000 b2sim-2.1.4/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0        0        0        0 2024-04-12 03:42:27.876385 b2sim-2.1.4/b2sim.egg-info/
--rw-rw-rw-   0        0        0      385 2024-04-12 03:42:27.000000 b2sim-2.1.4/b2sim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2024-04-12 03:42:27.000000 b2sim-2.1.4/b2sim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 03:42:27.000000 b2sim-2.1.4/b2sim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-12 03:42:27.000000 b2sim-2.1.4/b2sim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 03:42:27.000000 b2sim-2.1.4/b2sim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 03:42:27.878460 b2sim-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0      488 2024-04-12 03:42:13.000000 b2sim-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.199327 b2sim-2.1.5/
+-rw-rw-rw-   0        0        0    35823 2023-05-09 05:51:58.000000 b2sim-2.1.5/LICENSE
+-rw-rw-rw-   0        0        0      123 2024-02-07 03:13:22.000000 b2sim-2.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2024-05-15 20:00:49.198328 b2sim-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    18853 2024-02-22 04:54:10.000000 b2sim-2.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.096504 b2sim-2.1.5/b2sim/
+-rw-rw-rw-   0        0        0        0 2024-02-05 03:29:23.000000 b2sim-2.1.5/b2sim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.142159 b2sim-2.1.5/b2sim/analysis/
+-rw-rw-rw-   0        0        0      108 2024-02-12 21:33:54.000000 b2sim-2.1.5/b2sim/analysis/__init__.py
+-rw-rw-rw-   0        0        0    25122 2024-05-15 06:39:44.000000 b2sim-2.1.5/b2sim/analysis/ai.py
+-rw-rw-rw-   0        0        0     4346 2024-02-21 01:49:15.000000 b2sim-2.1.5/b2sim/analysis/fitness.py
+-rw-rw-rw-   0        0        0     5061 2024-02-12 21:30:11.000000 b2sim-2.1.5/b2sim/analysis/graphing.py
+-rw-rw-rw-   0        0        0     5674 2024-02-07 01:42:59.000000 b2sim-2.1.5/b2sim/analysis/visualize.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.178679 b2sim-2.1.5/b2sim/engine/
+-rw-rw-rw-   0        0        0      102 2024-02-04 07:54:08.000000 b2sim-2.1.5/b2sim/engine/__init__.py
+-rw-rw-rw-   0        0        0    14197 2024-02-23 22:29:57.000000 b2sim-2.1.5/b2sim/engine/actions.py
+-rw-rw-rw-   0        0        0    13545 2024-05-15 06:56:28.000000 b2sim-2.1.5/b2sim/engine/farms.py
+-rw-rw-rw-   0        0        0     9918 2024-02-08 21:25:01.000000 b2sim-2.1.5/b2sim/engine/info.py
+-rw-rw-rw-   0        0        0   102973 2024-05-09 00:56:22.000000 b2sim-2.1.5/b2sim/engine/main.py
+-rw-rw-rw-   0        0        0     5069 2024-02-09 00:43:24.000000 b2sim-2.1.5/b2sim/engine/rounds.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.195814 b2sim-2.1.5/b2sim/templates/
+-rw-rw-rw-   0        0        0     1944 2024-02-19 06:29:12.000000 b2sim-2.1.5/b2sim/templates/config.txt
+-rw-rw-rw-   0        0        0     2027 2024-04-12 03:06:06.000000 b2sim-2.1.5/b2sim/templates/eco_send_info.csv
+-rw-rw-rw-   0        0        0      613 2023-07-19 19:03:45.000000 b2sim-2.1.5/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.197318 b2sim-2.1.5/b2sim.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-05-15 20:00:49.000000 b2sim-2.1.5/b2sim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2024-05-15 20:00:49.000000 b2sim-2.1.5/b2sim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:00:49.000000 b2sim-2.1.5/b2sim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-15 20:00:49.000000 b2sim-2.1.5/b2sim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 20:00:49.000000 b2sim-2.1.5/b2sim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:00:49.199327 b2sim-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      469 2024-05-15 06:35:31.000000 b2sim-2.1.5/setup.py
```

### Comparing `b2sim-2.1.4/LICENSE` & `b2sim-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.4/README.md` & `b2sim-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.4/b2sim/analysis/ai.py` & `b2sim-2.1.5/b2sim/analysis/ai.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,520 +1,520 @@
-import neat
-import b2sim.engine as b2
-from copy import deepcopy as dc
-import os
-from bisect import bisect_left
-from math import floor, ceil
-
-class AI():
-    '''
-    A class for training neural networks using the NEAT method to optimize farming
-    strategies in Battles 2.
-    '''
-
-    def __init__(self, initial_state_game):
-        self.initial_state_game = initial_state_game
-
-        self.net = None # The neural network that the AI will use to make important decisions
-        self.game_state = None # The game state associated with the AI   
-        self.max_farms = 5
-        self.buy_factor = 0
-
-        # Used to penalize the AI for making obviously suboptimal decisions. Starts at 1 and decreases every time an error is made
-        self.fitness_multiplier = 1
-        self.penalty_intensity = 0.01
-
-        # If the user wants to train the AI with constraints applied to the eco and buy queues, 
-        # they can apply those constraints via these varaibles
-        self.fixed_eco_queue = []
-        self.fixed_buy_queue = []
-
-        self.decision_history = [] # List of dict objects which keeps track of key decisions the AI makes throughout simulation
-        self.actions_list_base = [] #A list of all outright farm purchases the AI could choose to make
-        self.farm_incomes = {} # Lists out per round incomes of all farms
-
-        for key in b2.farm_payout_values.keys():
-            ppr = b2.farm_payout_values[key][0]*b2.farm_payout_values[key][1]
-            if key[2] == 5:
-                #Accounting for the MWS bonus
-                ppr += 10000
+# import neat
+# import b2sim.engine as b2
+# from copy import deepcopy as dc
+# import os
+# from bisect import bisect_left
+# from math import floor, ceil
+
+# class AI():
+#     '''
+#     A class for training neural networks using the NEAT method to optimize farming
+#     strategies in Battles 2.
+#     '''
+
+#     def __init__(self, initial_state_game):
+#         self.initial_state_game = initial_state_game
+
+#         self.net = None # The neural network that the AI will use to make important decisions
+#         self.game_state = None # The game state associated with the AI   
+#         self.max_farms = 5
+#         self.buy_factor = 0
+
+#         # Used to penalize the AI for making obviously suboptimal decisions. Starts at 1 and decreases every time an error is made
+#         self.fitness_multiplier = 1
+#         self.penalty_intensity = 0.01
+
+#         # If the user wants to train the AI with constraints applied to the eco and buy queues, 
+#         # they can apply those constraints via these varaibles
+#         self.fixed_eco_queue = []
+#         self.fixed_buy_queue = []
+
+#         self.decision_history = [] # List of dict objects which keeps track of key decisions the AI makes throughout simulation
+#         self.actions_list_base = [] #A list of all outright farm purchases the AI could choose to make
+#         self.farm_incomes = {} # Lists out per round incomes of all farms
+
+#         for key in b2.farm_payout_values.keys():
+#             ppr = b2.farm_payout_values[key][0]*b2.farm_payout_values[key][1]
+#             if key[2] == 5:
+#                 #Accounting for the MWS bonus
+#                 ppr += 10000
             
-            if key[1] >= 3:
-                #Accounting for banks in particular
-                ppr = b2.farm_globals['Start of Round Bank Multiplier']*(ppr + b2.farm_globals['Start of Round Bank Payment'])
+#             if key[1] >= 3:
+#                 #Accounting for banks in particular
+#                 ppr = b2.farm_globals['Start of Round Bank Multiplier']*(ppr + b2.farm_globals['Start of Round Bank Payment'])
             
-            entry = {
-                'Type': 'Purchase',
-                'Upgrades': key,
-                'Income': ppr,
-                'Cost': b2.farm_total_cost_values[key]
-            }
-            self.actions_list_base.append(entry)
-            self.farm_incomes[key] = ppr
-
-        # The complete list of actions the AI considers throughout simulation
-        # At simulation start, this will just be outright farm buys, but as the simulation proceeds and the AI builds farms
-        # Decisions to upgrade farms or sell into higher tier farms will show up in this list
-        self.actions_list = dc(self.actions_list_base) 
-
-        # Determine path to configuration file. This path manipulation is
-        # here so that the script will run successfully regardless of the
-        # current working directory.
-        self.config_path = os.path.dirname(__file__)
-        self.config_path = os.path.join(self.config_path, '..')
-        self.config_path = os.path.join(self.config_path, 'templates/config.txt')
-
-    def penalize(self):
-        if self.game_state is not None and len(self.game_state.time_states) > 1:
-            self.fitness_multiplier -= self.penalty_intensity*(self.game_state.time_states[-1] - self.game_state.time_states[-2])
+#             entry = {
+#                 'Type': 'Purchase',
+#                 'Upgrades': key,
+#                 'Income': ppr,
+#                 'Cost': b2.farm_total_cost_values[key]
+#             }
+#             self.actions_list_base.append(entry)
+#             self.farm_incomes[key] = ppr
+
+#         # The complete list of actions the AI considers throughout simulation
+#         # At simulation start, this will just be outright farm buys, but as the simulation proceeds and the AI builds farms
+#         # Decisions to upgrade farms or sell into higher tier farms will show up in this list
+#         self.actions_list = dc(self.actions_list_base) 
+
+#         # Determine path to configuration file. This path manipulation is
+#         # here so that the script will run successfully regardless of the
+#         # current working directory.
+#         self.config_path = os.path.dirname(__file__)
+#         self.config_path = os.path.join(self.config_path, '..')
+#         self.config_path = os.path.join(self.config_path, 'templates/config.txt')
+
+#     def penalize(self):
+#         if self.game_state is not None and len(self.game_state.time_states) > 1:
+#             self.fitness_multiplier -= self.penalty_intensity*(self.game_state.time_states[-1] - self.game_state.time_states[-2])
         
-    def train(self, target_time, fitness_function, fitness_parameters, increment_value = 6.0, num_generations = 50, log = False):
-        '''
-        Train the AI on its assigned initial_game_state and a given target time.
+#     def train(self, target_time, fitness_function, fitness_parameters, increment_value = 6.0, num_generations = 50, log = False):
+#         '''
+#         Train the AI on its assigned initial_game_state and a given target time.
         
-        Parameters:
-        target_time (float): The time to simulate to
-        fitness_function (func): A function that will be used to evaluate the effectiveness of the AI
-        fitness_parameters (Dict): Parameters for the fitness function
-        increment_value (float): Determines how long each step in the simulation is.
-        num_generations (int): Determines how many epochs to run
-        '''
-
-        # Load configuration.
-        config = neat.Config(neat.DefaultGenome, neat.DefaultReproduction,
-                            neat.DefaultSpeciesSet, neat.DefaultStagnation,
-                            self.config_path)
-
-        # Create the population, which is the top-level object for a NEAT run.
-        p = neat.Population(config)
-
-        # Add a stdout reporter to show progress in the terminal.
-        p.add_reporter(neat.StdOutReporter(True))
-        stats = neat.StatisticsReporter()
-        p.add_reporter(stats)
-        p.add_reporter(neat.Checkpointer(5))
+#         Parameters:
+#         target_time (float): The time to simulate to
+#         fitness_function (func): A function that will be used to evaluate the effectiveness of the AI
+#         fitness_parameters (Dict): Parameters for the fitness function
+#         increment_value (float): Determines how long each step in the simulation is.
+#         num_generations (int): Determines how many epochs to run
+#         '''
+
+#         # Load configuration.
+#         config = neat.Config(neat.DefaultGenome, neat.DefaultReproduction,
+#                             neat.DefaultSpeciesSet, neat.DefaultStagnation,
+#                             self.config_path)
+
+#         # Create the population, which is the top-level object for a NEAT run.
+#         p = neat.Population(config)
+
+#         # Add a stdout reporter to show progress in the terminal.
+#         p.add_reporter(neat.StdOutReporter(True))
+#         stats = neat.StatisticsReporter()
+#         p.add_reporter(stats)
+#         p.add_reporter(neat.Checkpointer(5))
 
-        def eval(genomes, config):
-            self.evalGenomes(genomes, config, target_time, increment_value, fitness_function, fitness_parameters, log = log)
+#         def eval(genomes, config):
+#             self.evalGenomes(genomes, config, target_time, increment_value, fitness_function, fitness_parameters, log = log)
         
-        # Run for up to 300 generations.
-        winner = p.run(eval, num_generations)
+#         # Run for up to 300 generations.
+#         winner = p.run(eval, num_generations)
 
-        # Display the winning genome.
-        print('\nBest genome:\n{!s}'.format(winner))
+#         # Display the winning genome.
+#         print('\nBest genome:\n{!s}'.format(winner))
 
-        # Show output of the most fit genome against training data.
-        print('\nOutput:')
-        self.net = neat.nn.FeedForwardNetwork.create(winner, config)
+#         # Show output of the most fit genome against training data.
+#         print('\nOutput:')
+#         self.net = neat.nn.FeedForwardNetwork.create(winner, config)
         
-        # How much fitness did the winning genome achieve?
-        winner_fitness = self.processGenome(winner, config, target_time, increment_value, fitness_function, fitness_parameters)
-        print("The winning network achieved a fitness of %s"%(winner_fitness))
+#         # How much fitness did the winning genome achieve?
+#         winner_fitness = self.processGenome(winner, config, target_time, increment_value, fitness_function, fitness_parameters)
+#         print("The winning network achieved a fitness of %s"%(winner_fitness))
 
     
-    def evalGenomes(self, genomes, config, target_time, increment_value, fitness_function, fitness_parameters, log = False):
-        for genome_id, genome in genomes:
-            genome.fitness = self.processGenome(genome, config, target_time, increment_value, fitness_function, fitness_parameters)
-            if log:
-                print("Genome %s achieved fitness %s with a fitness x'er of %s and final eco %s"%(genome_id, genome.fitness, self.fitness_multiplier, self.game_state.eco))
-
-    def processGenome(self, genome, config, target_time, increment_value, fitness_function, fitness_parameters):
-        '''
-        Determine the fitness of a given genome.
-
-        Returns:
-        fitness (float): A rating of how well the genome performed
-        '''
-        # From the neural network we'll use to simulate from the genome and config info
-        net = neat.nn.FeedForwardNetwork.create(genome, config)
-
-        # Reset the fitness multiplier
-        self.fitness_multiplier = 1
-
-        # Run a simulation to the target time using the neural network
-        self.simulate(target_time, increment_value, neural_net = net, log = False)
-
-        # Evaluate the fitness of the AI
-        if self.fitness_multiplier < 0:
-            self.fitness_multiplier = 0
-
-        return self.fitness_multiplier*fitness_function(self.game_state, fitness_parameters)
-
-    def simulate(self, target_time, increment_value = 6, max_farms = 5, neural_net = None, log = True):
-        '''
-        Simulate a GameState from its current time to the target time by having the neural network automatically
-        determine what actions to take during the simulation.
-
-        It is recommended to disable the logger during training
-        '''
-
-        self.game_state = b2.GameState(dc(self.initial_state_game))
-        self.actions_list = []
-        self.getActions()
-
-        # Default to using the class-specified neural network if none is specified
-        if neural_net is None:
-            neural_net = self.net
+#     def evalGenomes(self, genomes, config, target_time, increment_value, fitness_function, fitness_parameters, log = False):
+#         for genome_id, genome in genomes:
+#             genome.fitness = self.processGenome(genome, config, target_time, increment_value, fitness_function, fitness_parameters)
+#             if log:
+#                 print("Genome %s achieved fitness %s with a fitness x'er of %s and final eco %s"%(genome_id, genome.fitness, self.fitness_multiplier, self.game_state.eco))
+
+#     def processGenome(self, genome, config, target_time, increment_value, fitness_function, fitness_parameters):
+#         '''
+#         Determine the fitness of a given genome.
+
+#         Returns:
+#         fitness (float): A rating of how well the genome performed
+#         '''
+#         # From the neural network we'll use to simulate from the genome and config info
+#         net = neat.nn.FeedForwardNetwork.create(genome, config)
+
+#         # Reset the fitness multiplier
+#         self.fitness_multiplier = 1
+
+#         # Run a simulation to the target time using the neural network
+#         self.simulate(target_time, increment_value, neural_net = net, log = False)
+
+#         # Evaluate the fitness of the AI
+#         if self.fitness_multiplier < 0:
+#             self.fitness_multiplier = 0
+
+#         return self.fitness_multiplier*fitness_function(self.game_state, fitness_parameters)
+
+#     def simulate(self, target_time, increment_value = 6, max_farms = 5, neural_net = None, log = True):
+#         '''
+#         Simulate a GameState from its current time to the target time by having the neural network automatically
+#         determine what actions to take during the simulation.
+
+#         It is recommended to disable the logger during training
+#         '''
+
+#         self.game_state = b2.GameState(dc(self.initial_state_game))
+#         self.actions_list = []
+#         self.getActions()
+
+#         # Default to using the class-specified neural network if none is specified
+#         if neural_net is None:
+#             neural_net = self.net
         
-        # Initialize the list of actions the AI can take throughout the simulation
-        old_info = None
+#         # Initialize the list of actions the AI can take throughout the simulation
+#         old_info = None
 
-        if log:
-            self.decision_history = []
-            self.eco_intensity_states = []
-            self.farm_intensity_states = []
-            self.time_states = []
-
-        while self.game_state.current_time < target_time:
-            # Pass the current game info through the genome, giving it the chance to process and spit out an output
-
-            # Parameter descriptions:
-            # CASH
-            # ECO
-            # FARM INCOME
-            # CURRENT TIME
-
-            # Using the parameters recorded from the previous self.self.game_state, determine the change in cash, eco, and farm_income
-            farm_income = farmIncome(self.game_state)
-
-            # if old_info is None:
-            #     old_info = {
-            #         'Cash': self.game_state.cash,
-            #         'Eco': self.game_state.eco,
-            #         'Farms': farmIncome(self.game_state)
-            #     }
-
-            # delta_cash = self.game_state.cash - old_info['Cash']
-            # delta_eco = self.game_state.eco - old_info['Eco']
-            # delta_farms = farm_income - old_info['Farms']
-
-            current_time = self.game_state.current_time
-            # current_round = self.game_state.rounds.getRoundFromTime(current_time)
-            # times_ahead = [self.game_state.rounds.getTimeFromRound(current_round + 1 + i) - current_time for i in range(3)]
-
-            output = neural_net.activate((self.game_state.cash, self.game_state.eco, farm_income, current_time))
-            eco_intensity, buy_signal = 20*output[0], 0.01*output[1]
-
-            # self.buy_factor += buy_signal*(6/increment_value)
-
-            if log:
-                self.eco_intensity_states.append(output[0])
-                self.farm_intensity_states.append(output[1])
-                self.time_states.append(self.game_state.current_time)
-
-            # What eco send should we use next?
-            available_sends = efficientFrontier(self.game_state.available_sends)
-            eco_send = self.determineEcoSend(eco_intensity, available_sends)
-            if self.game_state.send_name != eco_send:
-                self.penalize()
-                self.game_state.eco_queue.append(b2.ecoSend(send_name = eco_send))
-
-            # What farm should we be pursuing?
-            def takeAction(game_state, recommended_action):
-                if len(game_state.buy_queue) == 0:
-                    game_state.buy_queue.append(recommended_action)
-                elif len(game_state.buy_queue) > 0 and recommended_action != self.game_state.buy_queue[0]:
-                    game_state.buy_queue[0] = recommended_action
-                return game_state
-
-            action_dict = self.determineAction(0.1-buy_signal, log = log)
-
-            if action_dict is not None:
-                if action_dict['Type'] == 'Purchase':
-                    # Identify the type of farm we intend to purchase and amend that to the queue
-                    recommended_action = [b2.buyFarm(upgrades=tuple(action_dict['Upgrades']))]
-                    self.game_state = takeAction(self.game_state, recommended_action)
-                elif action_dict['Type'] == 'Upgrade':
-                    # The action type is an upgrade. Identify which farm is to be upgraded, then append the action to the queue
-                    # print("Upgrading farm at index %s to (%s,%s,%s)"%(action_dict['Index'], action_dict['Upgrades'][0],action_dict['Upgrades'][1],action_dict['Upgrades'][2]))
-                    # print(self.game_state.farms)
-                    recommended_action = [b2.upgradeFarm(index=action_dict['Index'], upgrades=tuple(action_dict['Upgrades']))]
-                    self.game_state = takeAction(self.game_state, recommended_action)
-                else:
-                    # The action type is a COMPOUND upgrade.
-                    # First, identify the farms to sell
-                    # print("Selling the first %s farms to upgrade farm at index %s to (%s,%s,%s)"%(action_dict['Farms To Sell'],action_dict['Index'], action_dict['Upgrades'][0],action_dict['Upgrades'][1],action_dict['Upgrades'][2]))
-                    # print(self.game_state.farms)
-                    recommended_action = [b2.sellFarm(index=k) for k in range(action_dict['Farms To Sell'])]
-                    recommended_action.append(b2.upgradeFarm(index=action_dict['Index'], upgrades=tuple(action_dict['Upgrades'])))
-                    self.game_state = takeAction(self.game_state, recommended_action)
+#         if log:
+#             self.decision_history = []
+#             self.eco_intensity_states = []
+#             self.farm_intensity_states = []
+#             self.time_states = []
+
+#         while self.game_state.current_time < target_time:
+#             # Pass the current game info through the genome, giving it the chance to process and spit out an output
+
+#             # Parameter descriptions:
+#             # CASH
+#             # ECO
+#             # FARM INCOME
+#             # CURRENT TIME
+
+#             # Using the parameters recorded from the previous self.self.game_state, determine the change in cash, eco, and farm_income
+#             farm_income = farmIncome(self.game_state)
+
+#             # if old_info is None:
+#             #     old_info = {
+#             #         'Cash': self.game_state.cash,
+#             #         'Eco': self.game_state.eco,
+#             #         'Farms': farmIncome(self.game_state)
+#             #     }
+
+#             # delta_cash = self.game_state.cash - old_info['Cash']
+#             # delta_eco = self.game_state.eco - old_info['Eco']
+#             # delta_farms = farm_income - old_info['Farms']
+
+#             current_time = self.game_state.current_time
+#             # current_round = self.game_state.rounds.getRoundFromTime(current_time)
+#             # times_ahead = [self.game_state.rounds.getTimeFromRound(current_round + 1 + i) - current_time for i in range(3)]
+
+#             output = neural_net.activate((self.game_state.cash, self.game_state.eco, farm_income, current_time))
+#             eco_intensity, buy_signal = 20*output[0], 0.01*output[1]
+
+#             # self.buy_factor += buy_signal*(6/increment_value)
+
+#             if log:
+#                 self.eco_intensity_states.append(output[0])
+#                 self.farm_intensity_states.append(output[1])
+#                 self.time_states.append(self.game_state.current_time)
+
+#             # What eco send should we use next?
+#             available_sends = efficientFrontier(self.game_state.available_sends)
+#             eco_send = self.determineEcoSend(eco_intensity, available_sends)
+#             if self.game_state.send_name != eco_send:
+#                 self.penalize()
+#                 self.game_state.eco_queue.append(b2.ecoSend(send_name = eco_send))
+
+#             # What farm should we be pursuing?
+#             def takeAction(game_state, recommended_action):
+#                 if len(game_state.buy_queue) == 0:
+#                     game_state.buy_queue.append(recommended_action)
+#                 elif len(game_state.buy_queue) > 0 and recommended_action != self.game_state.buy_queue[0]:
+#                     game_state.buy_queue[0] = recommended_action
+#                 return game_state
+
+#             action_dict = self.determineAction(0.1-buy_signal, log = log)
+
+#             if action_dict is not None:
+#                 if action_dict['Type'] == 'Purchase':
+#                     # Identify the type of farm we intend to purchase and amend that to the queue
+#                     recommended_action = [b2.buyFarm(upgrades=tuple(action_dict['Upgrades']))]
+#                     self.game_state = takeAction(self.game_state, recommended_action)
+#                 elif action_dict['Type'] == 'Upgrade':
+#                     # The action type is an upgrade. Identify which farm is to be upgraded, then append the action to the queue
+#                     # print("Upgrading farm at index %s to (%s,%s,%s)"%(action_dict['Index'], action_dict['Upgrades'][0],action_dict['Upgrades'][1],action_dict['Upgrades'][2]))
+#                     # print(self.game_state.farms)
+#                     recommended_action = [b2.upgradeFarm(index=action_dict['Index'], upgrades=tuple(action_dict['Upgrades']))]
+#                     self.game_state = takeAction(self.game_state, recommended_action)
+#                 else:
+#                     # The action type is a COMPOUND upgrade.
+#                     # First, identify the farms to sell
+#                     # print("Selling the first %s farms to upgrade farm at index %s to (%s,%s,%s)"%(action_dict['Farms To Sell'],action_dict['Index'], action_dict['Upgrades'][0],action_dict['Upgrades'][1],action_dict['Upgrades'][2]))
+#                     # print(self.game_state.farms)
+#                     recommended_action = [b2.sellFarm(index=k) for k in range(action_dict['Farms To Sell'])]
+#                     recommended_action.append(b2.upgradeFarm(index=action_dict['Index'], upgrades=tuple(action_dict['Upgrades'])))
+#                     self.game_state = takeAction(self.game_state, recommended_action)
                 
-            # Finally, run the simulation for some time
-            # When doing so, check whether or not ANY information about the game state's farms changes.
-            # If it does, update the list of ai_actions
+#             # Finally, run the simulation for some time
+#             # When doing so, check whether or not ANY information about the game state's farms changes.
+#             # If it does, update the list of ai_actions
             
-            # Collecting variables representing the game's current state for future use
-            # old_info = {
-            #     'Cash': self.game_state.cash,
-            #     'Eco': self.game_state.eco,
-            #     'Farms': farmIncome(self.game_state),
-            # }
-            old_farms = dc(self.game_state.farms)
-            self.game_state.fastForward(target_time = min(self.game_state.current_time + increment_value, target_time))
-
-            farms_changed = False
-            if len(old_farms) != len(self.game_state.farms):
-                # If we bought a new farm...
-                # print("farms changed because of new farm buy")
-                farms_changed = True
-            else:
-                # Check that all farms are the same
-                for i in range(len(old_farms)):
-                    if old_farms[i] != self.game_state.farms[i]:
-                        farms_changed = True
-                        # print("farms changed because of an upgrade")
-                        break
+#             # Collecting variables representing the game's current state for future use
+#             # old_info = {
+#             #     'Cash': self.game_state.cash,
+#             #     'Eco': self.game_state.eco,
+#             #     'Farms': farmIncome(self.game_state),
+#             # }
+#             old_farms = dc(self.game_state.farms)
+#             self.game_state.fastForward(target_time = min(self.game_state.current_time + increment_value, target_time))
+
+#             farms_changed = False
+#             if len(old_farms) != len(self.game_state.farms):
+#                 # If we bought a new farm...
+#                 # print("farms changed because of new farm buy")
+#                 farms_changed = True
+#             else:
+#                 # Check that all farms are the same
+#                 for i in range(len(old_farms)):
+#                     if old_farms[i] != self.game_state.farms[i]:
+#                         farms_changed = True
+#                         # print("farms changed because of an upgrade")
+#                         break
             
-            if farms_changed:
-                self.game_state.sortFarms(debug = False)
-                self.getActions()
+#             if farms_changed:
+#                 self.game_state.sortFarms(debug = False)
+#                 self.getActions()
     
-    def determineAction(self, cost_penalty = 0, log = False):
-        '''
-        Given an amount of a cash and a sorted list of actions to take, determine the *best* action to take and return that action.
-        The best action is determined by the income the action provides minus a penalty given to cost.
-        The penalty increases as cost increases and the penalty intensity is determined by cost_penalty.
-
-        Parameters:
-        ai_actions (List[Dict]): A list of dict objects describing feasible actions the AI could take
-        cost_penalty (float)
-
-        Returns:
-        Dict
-        '''
-        cash = self.game_state.cash
-        if len(self.game_state.eco_queue) > 0:
-            cash -= b2.eco_send_info[self.game_state.eco_queue[0]['Send Name']]['Price']
-        else:
-            cash -= self.game_state.eco_cost
-
-        def util(x):
-            if cash < x['Cost']:
-                # Any actions we can't afford should not be considered at all
-                return -1*float('inf')
-            elif x['Cost'] > 0:
-                # How to rate actions we can afford
-                return x['Income'] - cost_penalty*(x['Cost'])**2
-            else:
-                # If an action has *negative* cost, it is always worth taking
-                return float('inf')
-
-        # utilities = list(map(util, self.actions_list))
-        self.actions_list.sort(key=lambda x : util(x))
-        decision_utility = util(self.actions_list[-1])
-        if decision_utility < 0:
-            return None
-
-        if log:
-            self.decision_history.append({
-                'Time': self.game_state.current_time,
-                'Cash': cash, 
-                'Eco': self.game_state.eco,
-                'Farms': dc(self.game_state.farms),
-                'Cost Penalty': cost_penalty,
-                'Decision Utility': decision_utility,
-                'Decision': self.actions_list[-1],
-                # 'Actions List': dc(self.actions_list)
-            })
-
-        return_val = self.actions_list[-1]
-
-        if log: 
-            pass
-            # print("Determined action: ")
-            # print(return_val)
-            # print("The current farms with this action are: ")
-            # print(self.game_state.farms)
+#     def determineAction(self, cost_penalty = 0, log = False):
+#         '''
+#         Given an amount of a cash and a sorted list of actions to take, determine the *best* action to take and return that action.
+#         The best action is determined by the income the action provides minus a penalty given to cost.
+#         The penalty increases as cost increases and the penalty intensity is determined by cost_penalty.
+
+#         Parameters:
+#         ai_actions (List[Dict]): A list of dict objects describing feasible actions the AI could take
+#         cost_penalty (float)
+
+#         Returns:
+#         Dict
+#         '''
+#         cash = self.game_state.cash
+#         if len(self.game_state.eco_queue) > 0:
+#             cash -= b2.eco_send_info[self.game_state.eco_queue[0]['Send Name']]['Price']
+#         else:
+#             cash -= self.game_state.eco_cost
+
+#         def util(x):
+#             if cash < x['Cost']:
+#                 # Any actions we can't afford should not be considered at all
+#                 return -1*float('inf')
+#             elif x['Cost'] > 0:
+#                 # How to rate actions we can afford
+#                 return x['Income'] - cost_penalty*(x['Cost'])**2
+#             else:
+#                 # If an action has *negative* cost, it is always worth taking
+#                 return float('inf')
+
+#         # utilities = list(map(util, self.actions_list))
+#         self.actions_list.sort(key=lambda x : util(x))
+#         decision_utility = util(self.actions_list[-1])
+#         if decision_utility < 0:
+#             return None
+
+#         if log:
+#             self.decision_history.append({
+#                 'Time': self.game_state.current_time,
+#                 'Cash': cash, 
+#                 'Eco': self.game_state.eco,
+#                 'Farms': dc(self.game_state.farms),
+#                 'Cost Penalty': cost_penalty,
+#                 'Decision Utility': decision_utility,
+#                 'Decision': self.actions_list[-1],
+#                 # 'Actions List': dc(self.actions_list)
+#             })
+
+#         return_val = self.actions_list[-1]
+
+#         if log: 
+#             pass
+#             # print("Determined action: ")
+#             # print(return_val)
+#             # print("The current farms with this action are: ")
+#             # print(self.game_state.farms)
 
-        return return_val
+#         return return_val
     
-    def getActions(self, debug = False):
-        '''
-        Update the list of suitable actions the AI can perform.
-
-        Returns:
-        None (Updates self.actions_list)
-        '''
-
-        # Count the number of active farms
-        active_farms = 0
-        while active_farms < len(self.game_state.farms) and self.game_state.farms[active_farms].sell_time is None:
-            active_farms += 1
+#     def getActions(self, debug = False):
+#         '''
+#         Update the list of suitable actions the AI can perform.
+
+#         Returns:
+#         None (Updates self.actions_list)
+#         '''
+
+#         # Count the number of active farms
+#         active_farms = 0
+#         while active_farms < len(self.game_state.farms) and self.game_state.farms[active_farms].sell_time is None:
+#             active_farms += 1
         
-        if active_farms < self.max_farms:
-            self.actions_list = dc(self.actions_list_base)
-        else:
-            self.actions_list = []
+#         if active_farms < self.max_farms:
+#             self.actions_list = dc(self.actions_list_base)
+#         else:
+#             self.actions_list = []
 
-        for h in range(active_farms):
+#         for h in range(active_farms):
             
-            if debug:
-                print("Considering farm %s"%(h))
-            farm = self.game_state.farms[h]
-            for i in range(3):
-                # Check if the AI has the option to upgrade the ith crosspath of the given farm or not.
-                # If they do, create a new farm action and append it to arr
-
-                # Is the farm's target path not yet T5?
-                if farm.upgrades[i] < 5:
-                    # Yes, it is!
+#             if debug:
+#                 print("Considering farm %s"%(h))
+#             farm = self.game_state.farms[h]
+#             for i in range(3):
+#                 # Check if the AI has the option to upgrade the ith crosspath of the given farm or not.
+#                 # If they do, create a new farm action and append it to arr
+
+#                 # Is the farm's target path not yet T5?
+#                 if farm.upgrades[i] < 5:
+#                     # Yes, it is!
                     
-                    # Is it a T3 elsewhere?
-                    # Are BOTH the other paths upgraded?
-                    T3_elsewhere = False
-                    both_upgraded = True
-                    for j in range(3):
-                        if j != i and farm.upgrades[j] >= 3:
-                            T3_elsewhere = True
-                            break
-                        if j != i and farm.upgrades[j] == 0:
-                            both_upgraded = False
+#                     # Is it a T3 elsewhere?
+#                     # Are BOTH the other paths upgraded?
+#                     T3_elsewhere = False
+#                     both_upgraded = True
+#                     for j in range(3):
+#                         if j != i and farm.upgrades[j] >= 3:
+#                             T3_elsewhere = True
+#                             break
+#                         if j != i and farm.upgrades[j] == 0:
+#                             both_upgraded = False
                     
-                    if (farm.upgrades[i] < 2 or (farm.upgrades[i] >= 2 and not T3_elsewhere)) and (not both_upgraded):
-                        # Build the entry and append it to AI actions_base
-                        new_upgrades = dc(farm.upgrades)
-                        new_upgrades[i] += 1
-                        ppr = self.farm_incomes[tuple(new_upgrades)] - self.farm_incomes[tuple(farm.upgrades)] 
-                        cost = b2.farm_upgrades_costs[i][farm.upgrades[i]]
-                        entry = {
-                            'Type': 'Upgrade',
-                            'Index': h,
-                            'Upgrades': tuple(new_upgrades),
-                            'Income': ppr,
-                            'Cost': cost
-                        }
-                        self.actions_list.append(entry)
-
-                        # TODO: If the farm is the most expensive farm currently held, OR if the farm is a T4 farm,
-                        # AND we are trying to upgrade the farm's main path...
-                        # Construct additional entries that involve selling less expensive farms to fund this upgrade.
-                        if h == (active_farms - 1) or farm.upgrades[i] >=3:
-                            if farm.sell_time is None:
-                                for k in range(h):
-                                    # Determine the impact of selling the cheapest k farms to fund the upgrade of the target farm
-
-                                    #if farms[k].revenue + b2.farm_sellback_values[tuple(farms[k].upgrades)] < b2.farm_total_cost_values[tuple(farms[k].upgrades)]:
-                                    #    break
-
-                                    ppr -= self.farm_incomes[tuple(self.game_state.farms[k].upgrades)]
-                                    cost -= b2.farm_sellback_values[tuple(self.game_state.farms[k].upgrades)]
-
-                                    entry = {
-                                        'Type': 'Compound Upgrade',
-                                        'Index': h,
-                                        'Farms To Sell': k+1,
-                                        'Upgrades': tuple(new_upgrades),
-                                        'Income': ppr,
-                                        'Cost': cost
-                                    }
+#                     if (farm.upgrades[i] < 2 or (farm.upgrades[i] >= 2 and not T3_elsewhere)) and (not both_upgraded):
+#                         # Build the entry and append it to AI actions_base
+#                         new_upgrades = dc(farm.upgrades)
+#                         new_upgrades[i] += 1
+#                         ppr = self.farm_incomes[tuple(new_upgrades)] - self.farm_incomes[tuple(farm.upgrades)] 
+#                         cost = b2.farm_upgrades_costs[i][farm.upgrades[i]]
+#                         entry = {
+#                             'Type': 'Upgrade',
+#                             'Index': h,
+#                             'Upgrades': tuple(new_upgrades),
+#                             'Income': ppr,
+#                             'Cost': cost
+#                         }
+#                         self.actions_list.append(entry)
+
+#                         # TODO: If the farm is the most expensive farm currently held, OR if the farm is a T4 farm,
+#                         # AND we are trying to upgrade the farm's main path...
+#                         # Construct additional entries that involve selling less expensive farms to fund this upgrade.
+#                         if h == (active_farms - 1) or farm.upgrades[i] >=3:
+#                             if farm.sell_time is None:
+#                                 for k in range(h):
+#                                     # Determine the impact of selling the cheapest k farms to fund the upgrade of the target farm
+
+#                                     #if farms[k].revenue + b2.farm_sellback_values[tuple(farms[k].upgrades)] < b2.farm_total_cost_values[tuple(farms[k].upgrades)]:
+#                                     #    break
+
+#                                     ppr -= self.farm_incomes[tuple(self.game_state.farms[k].upgrades)]
+#                                     cost -= b2.farm_sellback_values[tuple(self.game_state.farms[k].upgrades)]
+
+#                                     entry = {
+#                                         'Type': 'Compound Upgrade',
+#                                         'Index': h,
+#                                         'Farms To Sell': k+1,
+#                                         'Upgrades': tuple(new_upgrades),
+#                                         'Income': ppr,
+#                                         'Cost': cost
+#                                     }
 
-                                    if entry['Income'] > 0:
-                                        self.actions_list.append(entry)
+#                                     if entry['Income'] > 0:
+#                                         self.actions_list.append(entry)
                         
 
-        # self.actions_list = pruneActions(self.actions_list)
-        self.actions_list.sort(key=lambda x: x['Cost'])
+#         # self.actions_list = pruneActions(self.actions_list)
+#         self.actions_list.sort(key=lambda x: x['Cost'])
 
-    def determineEcoSend(self, intensity, eco_sends):
-        ind = bisect_left(eco_sends, intensity, key = lambda send_name: b2.eco_send_info[send_name]['Eco Intensity']) - 1
+#     def determineEcoSend(self, intensity, eco_sends):
+#         ind = bisect_left(eco_sends, intensity, key = lambda send_name: b2.eco_send_info[send_name]['Eco Intensity']) - 1
 
-        send_name = None
-        if ind >= 0:
-            send_name = eco_sends[ind]
-        else:
-            send_name = eco_sends[0]
-
-        # If the AI picks an eco send that runs them out of money *and* there was a more efficient eco send available to choose...
-        # Penalize the AI for making this decision
-        next_eco_tick = 6*(floor(self.game_state.current_time/6) + 1)
-        if ind > 1 and self.game_state.cash < (next_eco_tick - self.game_state.current_time)*b2.eco_send_info[send_name]['Cost Intensity'] and len(self.game_state.time_states) > 1:
-            self.penalize()
+#         send_name = None
+#         if ind >= 0:
+#             send_name = eco_sends[ind]
+#         else:
+#             send_name = eco_sends[0]
+
+#         # If the AI picks an eco send that runs them out of money *and* there was a more efficient eco send available to choose...
+#         # Penalize the AI for making this decision
+#         next_eco_tick = 6*(floor(self.game_state.current_time/6) + 1)
+#         if ind > 1 and self.game_state.cash < (next_eco_tick - self.game_state.current_time)*b2.eco_send_info[send_name]['Cost Intensity'] and len(self.game_state.time_states) > 1:
+#             self.penalize()
 
-        return send_name
+#         return send_name
 
         
 
 
-def efficientFrontier(eco_sends):
-    '''
-    Given a list of eco sends, determine which ones belong to the efficient eco frontier
+# def efficientFrontier(eco_sends):
+#     '''
+#     Given a list of eco sends, determine which ones belong to the efficient eco frontier
     
-    Parameters:
-    eco_sends (List[str]): A list containing names of eco sends for consideration
+#     Parameters:
+#     eco_sends (List[str]): A list containing names of eco sends for consideration
 
-    Returns:
-    (List[str]): A list containing names of non-dominated pure eco sends
-    '''
-
-    # First, sort the sends based on cost intensity
-    eco_sends.sort(key = lambda send_name: b2.eco_send_info[send_name]['Cost Intensity'])
-
-    # Now determine the indices that correspond to eef sends
-    i = 0
-    eef = [0]
-    while i < len(eco_sends)-1:
+#     Returns:
+#     (List[str]): A list containing names of non-dominated pure eco sends
+#     '''
+
+#     # First, sort the sends based on cost intensity
+#     eco_sends.sort(key = lambda send_name: b2.eco_send_info[send_name]['Cost Intensity'])
+
+#     # Now determine the indices that correspond to eef sends
+#     i = 0
+#     eef = [0]
+#     while i < len(eco_sends)-1:
         
-        #Test remaining eco sends to determine which ones belong on the EEF
-        slope = 0
-        index = None
-        for j in range(i+1,len(eco_sends)):
-            test_num = b2.eco_send_info[eco_sends[j]]['Eco Intensity'] - b2.eco_send_info[eco_sends[i]]['Eco Intensity']
-            test_den = b2.eco_send_info[eco_sends[j]]['Cost Intensity'] - b2.eco_send_info[eco_sends[i]]['Cost Intensity']
-            test_val = test_num/test_den
-            #print("Test value for index (" + str(i) + ", " + str(j) + "): " + str(test_val))
-            if test_val > slope:
-                slope = test_val
-                index = j
+#         #Test remaining eco sends to determine which ones belong on the EEF
+#         slope = 0
+#         index = None
+#         for j in range(i+1,len(eco_sends)):
+#             test_num = b2.eco_send_info[eco_sends[j]]['Eco Intensity'] - b2.eco_send_info[eco_sends[i]]['Eco Intensity']
+#             test_den = b2.eco_send_info[eco_sends[j]]['Cost Intensity'] - b2.eco_send_info[eco_sends[i]]['Cost Intensity']
+#             test_val = test_num/test_den
+#             #print("Test value for index (" + str(i) + ", " + str(j) + "): " + str(test_val))
+#             if test_val > slope:
+#                 slope = test_val
+#                 index = j
                 
-        # When the correct index is discovered, append it to eef
-        if index is not None and index > i:
-            eef.append(index)
-            i = index
-        else:
-            #It is possible we may run out of eco sends to add to the frontier, in which case...
-            break
+#         # When the correct index is discovered, append it to eef
+#         if index is not None and index > i:
+#             eef.append(index)
+#             i = index
+#         else:
+#             #It is possible we may run out of eco sends to add to the frontier, in which case...
+#             break
         
-    return [eco_sends[ind] for ind in eef]
+#     return [eco_sends[ind] for ind in eef]
 
-def ecoIntensity(intensity: float, eco_sends):
-    '''
-    Given a desired eco intensity and a list of non-dominated eco_sends sorted in order of increasing intensity, 
-    determine the highest intensity eco send among all currently available that does not exceed the given desired eco intensity.
+# def ecoIntensity(intensity: float, eco_sends):
+#     '''
+#     Given a desired eco intensity and a list of non-dominated eco_sends sorted in order of increasing intensity, 
+#     determine the highest intensity eco send among all currently available that does not exceed the given desired eco intensity.
 
-    The eco intensity of an eco send is defined as the eco awarded divided by the amount of time it takes to send.
+#     The eco intensity of an eco send is defined as the eco awarded divided by the amount of time it takes to send.
     
-    Parameters:
-    intensity (float): The highest desired rate of eco gain (expressed in terms of eco gained per 6 seconds)
-    eco_sends (List[str]): A list of non-dominated eco sends to be considered, sorted in order of increasing cost intensity
-
-    Returns:
-    eco_send (str): A string which names an eco send and corresponds to an entry in the eco_send_info dictionary
-    '''
-    ind = bisect_left(eco_sends, intensity, key = lambda send_name: b2.eco_send_info[send_name]['Eco Intensity']) - 1
-    if ind >= 0:
-        return eco_sends[ind]
-    else:
-        return eco_sends[0]
+#     Parameters:
+#     intensity (float): The highest desired rate of eco gain (expressed in terms of eco gained per 6 seconds)
+#     eco_sends (List[str]): A list of non-dominated eco sends to be considered, sorted in order of increasing cost intensity
+
+#     Returns:
+#     eco_send (str): A string which names an eco send and corresponds to an entry in the eco_send_info dictionary
+#     '''
+#     ind = bisect_left(eco_sends, intensity, key = lambda send_name: b2.eco_send_info[send_name]['Eco Intensity']) - 1
+#     if ind >= 0:
+#         return eco_sends[ind]
+#     else:
+#         return eco_sends[0]
     
-def farmIncome(gs):
-    '''
-    Given a GameState class object, determine how much per round income the farms from that game_state object produces.
-    The per round income of banks is estimated by computing the payout it gives over 1 round when no money is held prior
-
-    Parameters:
-    gs (GameState): A GameState object
-
-    Returns:
-    (float): How much money the farms will generate 
-    '''
-
-    round_income = 0
-    for farm in gs.farms:
-        ppr = b2.farm_payout_values[tuple(farm.upgrades)][0]*b2.farm_payout_values[tuple(farm.upgrades)][1]
-        if gs.T5_exists[0] and farm.upgrades[0] == 4:
-            ppr = ppr*b2.farm_globals['Banana Central Multiplier']
-
-        round_income += ppr
-        if farm.upgrades[2] == 5:
-            round_income += 10000
+# def farmIncome(gs):
+#     '''
+#     Given a GameState class object, determine how much per round income the farms from that game_state object produces.
+#     The per round income of banks is estimated by computing the payout it gives over 1 round when no money is held prior
+
+#     Parameters:
+#     gs (GameState): A GameState object
+
+#     Returns:
+#     (float): How much money the farms will generate 
+#     '''
+
+#     round_income = 0
+#     for farm in gs.farms:
+#         ppr = b2.farm_payout_values[tuple(farm.upgrades)][0]*b2.farm_payout_values[tuple(farm.upgrades)][1]
+#         if gs.T5_exists[0] and farm.upgrades[0] == 4:
+#             ppr = ppr*b2.farm_globals['Banana Central Multiplier']
+
+#         round_income += ppr
+#         if farm.upgrades[2] == 5:
+#             round_income += 10000
 
-    return round_income
+#     return round_income
```

### Comparing `b2sim-2.1.4/b2sim/analysis/fitness.py` & `b2sim-2.1.5/b2sim/analysis/fitness.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.4/b2sim/analysis/graphing.py` & `b2sim-2.1.5/b2sim/analysis/graphing.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.4/b2sim/analysis/visualize.py` & `b2sim-2.1.5/b2sim/analysis/visualize.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.4/b2sim/engine/actions.py` & `b2sim-2.1.5/b2sim/engine/actions.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.4/b2sim/engine/info.py` & `b2sim-2.1.5/b2sim/engine/info.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.4/b2sim/engine/main.py` & `b2sim-2.1.5/b2sim/engine/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -959,121 +959,19 @@
                         'Payout': payout_amount,
                         'Source': 'Heli'
                     }
                     payout_times.append(payout_entry)
                     heli_farm_time += heli_globals['Heli Farm Usage Cooldown']
 
         #FARMS
-        if len(self.farms) > 0:
-            for key, farm in enumerate(self.farms):
-                if farm.sell_time is None:
-                    #If the farm is a monkeynomics, determine the payout times of the active ability
-                    if farm.upgrades[1] == 5:
-                        farm_time = farm.min_use_time
-                        while farm_time <= target_time:
-                            if farm_time > self.current_time:
-                                payout_entry = {
-                                    'Time': farm_time,
-                                    'Payout Type': 'Direct',
-                                    'Payout': farm_globals['Monkeynomics Payout'],
-                                    'Source': 'Farm',
-                                    'Index': key
-                                }
-                                payout_times.append(payout_entry)
-                            farm_time += farm_globals['Monkeynomics Usage Cooldown']
-                        farm.min_use_time = farm_time
-                    
-                    farm_purchase_round = self.rounds.getRoundFromTime(farm.purchase_time)
-                    self.inc = 0
-                    self.flag = False
-                    while self.flag == False:
-                        #If computing farm payments on the same round as we are currently on, precompute the indices the for loop should go through.
-                        #NOTE: This is not necessary at the end because the for loop terminates when a "future" payment is reached.
-                        if self.inc == 0:
-                            if self.current_round > farm_purchase_round:
-                                #When the farm was purchased on a previous round
-                                round_time = self.current_time - self.rounds.round_starts[self.current_round]
-                                loop_start = int(floor(farm.payout_frequency*round_time/self.rounds.nat_send_lens[self.current_round]) + 1)
-                                loop_end = farm.payout_frequency
-                            else: #self.current_round == farm_purhcase_round
-                                #When the farm was purchased on the same round as we are currently on
-                                loop_start = int(floor(farm.payout_frequency*(self.current_time - farm.purchase_time)/self.rounds.nat_send_lens[self.current_round]-1)+1)
-                                loop_end = int(ceil(farm.payout_frequency*(1 - (farm.purchase_time - self.rounds.round_starts[self.current_round])/self.rounds.nat_send_lens[self.current_round])-1)-1)
-                        else:
-                            loop_start = 0
-                            loop_end = farm.payout_frequency
-                        
-                        #self.logs.append("Precomputed the loop indices to be (%s,%s)"%(loop_start,loop_end))
-                        #self.logs.append("Now computing payments at round %s"%(self.current_round + self.inc))
-                        
-                        for i in range(loop_start, loop_end):
-                            #Precompute the value i that this for loop should start at (as opposed to always starting at 0) to avoid redundant computations
-                            #Farm payout rules are different for the round the farm is bought on versus subsequent rounds
-                            if self.current_round + self.inc == farm_purchase_round:
-                                farm_time = farm.purchase_time + (i+1)*self.rounds.nat_send_lens[self.current_round + self.inc]/farm.payout_frequency
-                            else:
-                                farm_time = self.rounds.round_starts[self.current_round + self.inc] + i*self.rounds.nat_send_lens[self.current_round + self.inc]/farm.payout_frequency
-                            
-                            #Check if the payment time occurs within our update window. If it does, add it to the payout times list
-                            if farm_time <= target_time and farm_time > self.current_time:
-                                
-                                #Farm payouts will either immediately be added to the player's cash or added to the monkey bank's account value
-                                #This depends of course on whether the farm is a bank or not.
-                                
-                                #WARNING: If the farm we are dealing with is a bank, we must direct the payment into the bank rather than the player.
-                                #WARNING: If the farm we are dealing with is a MWS, we must check whether we are awarding the MWS bonus payment!
-                                #WARNING: If the farm we are dealing with is a BRF, we must check whether the BRF buff is being applied or not!
-                                
-                                if farm.upgrades[1] >= 3:
-                                    if i == 0 and self.current_round + self.inc > farm_purchase_round:
-                                        #At the start of every round, every bank gets a $400 payment and then is awarded 20% interest.
-                                        payout_entry = {
-                                            'Time': farm_time,
-                                            'Payout Type': 'Bank Interest',
-                                            'Index': key,
-                                            'Source': 'Farm'
-                                        }
-                                        payout_times.append(payout_entry)
-                                    payout_entry = {
-                                        'Time': farm_time,
-                                        'Payout Type': 'Bank Payment',
-                                        'Index': key,
-                                        'Payout': farm.payout(farm_time),
-                                        'Source': 'Farm'
-                                    }
-                                elif i == 0 and farm.upgrades[2] == 5 and self.current_round + self.inc > farm_purchase_round:
-                                    payout_entry = {
-                                        'Time': farm_time,
-                                        'Payout Type': 'Direct',
-                                        'Payout': farm.payout(farm_time, mws_bonus = True),
-                                        'Source': 'Farm',
-                                        'Index': key
-                                    }
-                                elif farm.upgrades[0] == 4 and self.T5_exists[0] == True:
-                                    payout_entry = {
-                                        'Time': farm_time,
-                                        'Payout Type': 'Direct',
-                                        'Payout': farm.payout(farm_time, brf_buff = True),
-                                        'Source': 'Farm',
-                                        'Index': key
-                                    }
-                                else:
-                                    payout_entry = {
-                                        'Time': farm_time,
-                                        'Payout Type': 'Direct',
-                                        'Payout': farm.payout(farm_time),
-                                        'Source': 'Farm',
-                                        'Index': key
-                                    }
-                                payout_times.append(payout_entry)
-                            elif farm_time > target_time:
-                                #self.logs.append("The payout time of %s is too late! Excluding payout time!"%(farm_time))
-                                self.flag = True
-                                break
-                        self.inc += 1
+        for key, farm in enumerate(self.farms):
+            farm_payout_times = farm.computePayoutSchedule(self.current_time, target_time, self.rounds, self.T5_exists[0])
+            for farm_payout_entry in farm_payout_times:
+                farm_payout_entry['Index'] = key
+            payout_times.extend(farm_payout_times)
         
         #BOAT FARMS
         if len(self.boat_farms) > 0:
 
             #Is there a Trade Empire on screen right now? 
             if self.Tempire_exists == True:
                 #Yes, determine the buff to be applied to other boat farm payments.
```

### Comparing `b2sim-2.1.4/b2sim/engine/rounds.py` & `b2sim-2.1.5/b2sim/engine/rounds.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.4/b2sim/templates/config.txt` & `b2sim-2.1.5/b2sim/templates/config.txt`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.4/b2sim/templates/eco_send_info.csv` & `b2sim-2.1.5/b2sim/templates/eco_send_info.csv`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.4/b2sim/templates/nat_send_lengths.csv` & `b2sim-2.1.5/b2sim/templates/nat_send_lengths.csv`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.4/b2sim.egg-info/SOURCES.txt` & `b2sim-2.1.5/b2sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

