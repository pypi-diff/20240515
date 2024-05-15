# Comparing `tmp/spooling-0.0.3.tar.gz` & `tmp/spooling-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spooling-0.0.3.tar", last modified: Tue May 14 20:18:57 2024, max compression
+gzip compressed data, was "spooling-0.0.4.tar", last modified: Wed May 15 01:06:42 2024, max compression
```

## Comparing `spooling-0.0.3.tar` & `spooling-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.830631 spooling-0.0.3/
--rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 spooling-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 spooling-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 spooling-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      600 2024-05-14 20:18:57.829631 spooling-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-05-14 19:52:48.000000 spooling-0.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.775631 spooling-0.0.3/daiexperiments.egg-info/
--rw-rw-rw-   0        0        0      393 2024-05-14 07:40:34.000000 spooling-0.0.3/daiexperiments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 07:40:34.000000 spooling-0.0.3/daiexperiments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 07:40:34.000000 spooling-0.0.3/daiexperiments.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.781636 spooling-0.0.3/ishandaiexperiments.egg-info/
--rw-rw-rw-   0        0        0      289 2024-05-13 20:00:47.000000 spooling-0.0.3/ishandaiexperiments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 20:00:47.000000 spooling-0.0.3/ishandaiexperiments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-13 20:00:47.000000 spooling-0.0.3/ishandaiexperiments.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.790631 spooling-0.0.3/pooLing.egg-info/
--rw-rw-rw-   0        0        0      484 2024-05-14 20:00:32.000000 spooling-0.0.3/pooLing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 20:00:32.000000 spooling-0.0.3/pooLing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 20:00:32.000000 spooling-0.0.3/pooLing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 20:18:57.830631 spooling-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      701 2024-05-14 20:18:52.000000 spooling-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.794670 spooling-0.0.3/spooling/
--rw-rw-rw-   0        0        0      239 2024-05-14 20:17:25.000000 spooling-0.0.3/spooling/__init__.py
--rw-rw-rw-   0        0        0    20539 2024-05-14 20:00:19.000000 spooling-0.0.3/spooling/main.py
-drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.827636 spooling-0.0.3/spooling.egg-info/
--rw-rw-rw-   0        0        0      600 2024-05-14 20:18:57.000000 spooling-0.0.3/spooling.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      574 2024-05-14 20:18:57.000000 spooling-0.0.3/spooling.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 20:18:57.000000 spooling-0.0.3/spooling.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-14 20:18:57.000000 spooling-0.0.3/spooling.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 01:06:42.386401 spooling-0.0.4/
+-rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 spooling-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 spooling-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 spooling-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      600 2024-05-15 01:06:42.385400 spooling-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2024-05-14 19:52:48.000000 spooling-0.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 01:06:42.309481 spooling-0.0.4/daiexperiments.egg-info/
+-rw-rw-rw-   0        0        0      393 2024-05-14 07:40:34.000000 spooling-0.0.4/daiexperiments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 07:40:34.000000 spooling-0.0.4/daiexperiments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 07:40:34.000000 spooling-0.0.4/daiexperiments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 01:06:42.327400 spooling-0.0.4/ishandaiexperiments.egg-info/
+-rw-rw-rw-   0        0        0      289 2024-05-13 20:00:47.000000 spooling-0.0.4/ishandaiexperiments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 20:00:47.000000 spooling-0.0.4/ishandaiexperiments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-13 20:00:47.000000 spooling-0.0.4/ishandaiexperiments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 01:06:42.342449 spooling-0.0.4/pooLing.egg-info/
+-rw-rw-rw-   0        0        0      484 2024-05-14 20:00:32.000000 spooling-0.0.4/pooLing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 20:00:32.000000 spooling-0.0.4/pooLing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 20:00:32.000000 spooling-0.0.4/pooLing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 01:06:42.387402 spooling-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      701 2024-05-15 01:06:36.000000 spooling-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:06:42.362403 spooling-0.0.4/spooling/
+-rw-rw-rw-   0        0        0      239 2024-05-14 20:17:25.000000 spooling-0.0.4/spooling/__init__.py
+-rw-rw-rw-   0        0        0    28677 2024-05-15 01:06:29.000000 spooling-0.0.4/spooling/main.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:06:42.383434 spooling-0.0.4/spooling.egg-info/
+-rw-rw-rw-   0        0        0      600 2024-05-15 01:06:42.000000 spooling-0.0.4/spooling.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2024-05-15 01:06:42.000000 spooling-0.0.4/spooling.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 01:06:42.000000 spooling-0.0.4/spooling.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 01:06:42.000000 spooling-0.0.4/spooling.egg-info/top_level.txt
```

### Comparing `spooling-0.0.3/LICENSE.txt` & `spooling-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spooling-0.0.3/PKG-INFO` & `spooling-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spooling
-Version: 0.0.3
+Version: 0.0.4
 Summary: rl experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spooling-0.0.3/setup.py` & `spooling-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='spooling',
-  version='0.0.3',
+  version='0.0.4',
   description='rl experiments',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='S Ishan',
   author_email='is9678@srmist.edu.in',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `spooling-0.0.3/spooling/main.py` & `spooling-0.0.4/spooling/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -589,8 +589,275 @@
         print("Training finished.")
 
 if __name__ == "__main__":
     env = Environment()
     agent = SARSA(env.num_states, env.num_actions)
     agent.train(env, episodes=1000)
 """
+    return code
+
+def policy_iteration_heh():
+
+    code = """
+import numpy as np
+import gym
+
+def policy_iteration(env, gamma=0.9, theta=1e-5):
+    num_states = env.observation_space.n
+    num_actions = env.action_space.n
+    policy = np.ones((num_states, num_actions)) / num_actions
+
+    def policy_evaluation(policy):
+        V = np.zeros(num_states)
+        while True:
+            delta = 0
+            for s in range(num_states):
+                v = V[s]
+                V[s] = sum(policy[s][a] * sum(p * (r + gamma * V[s_]) for p, s_, r, _ in env.P[s][a]) for a in range(num_actions))
+                delta = max(delta, abs(v - V[s]))
+            if delta < theta:
+                break
+        return V
+
+    def policy_improvement(V):
+        new_policy = np.zeros((num_states, num_actions))
+        for s in range(num_states):
+            q_values = np.zeros(num_actions)
+            for a in range(num_actions):
+                q_values[a] = sum(p * (r + gamma * V[s_]) for p, s_, r, _ in env.P[s][a])
+            best_action = np.argmax(q_values)
+            new_policy[s][best_action] = 1
+        return new_policy
+
+    policy_stable = False
+    while not policy_stable:
+        V = policy_evaluation(policy)
+        new_policy = policy_improvement(V)
+        if np.array_equal(new_policy, policy):
+            policy_stable = True
+        policy = new_policy
+
+    return policy, V
+
+if __name__ == "__main__":
+    env = gym.make('FrozenLake-v1')
+    policy, V = policy_iteration(env)
+    print("Optimal Policy:")
+    print(policy)
+    print("Optimal Value Function:")
+    print(V)
+
+"""
+    return code
+
+def value_iteration_heh():
+
+    code = """
+import numpy as np
+import gym
+
+def value_iteration(env, gamma=0.9, theta=1e-5):
+    num_states = env.observation_space.n
+    num_actions = env.action_space.n
+    V = np.zeros(num_states)
+
+    def q_value(state, action):
+        return sum(p * (r + gamma * V[s_]) for p, s_, r, _ in env.P[state][action])
+
+    while True:
+        delta = 0
+        for s in range(num_states):
+            v = V[s]
+            V[s] = max(q_value(s, a) for a in range(num_actions))
+            delta = max(delta, abs(v - V[s]))
+        if delta < theta:
+            break
+
+    policy = np.zeros((num_states, num_actions))
+    for s in range(num_states):
+        q_values = [q_value(s, a) for a in range(num_actions)]
+        best_action = np.argmax(q_values)
+        policy[s][best_action] = 1
+
+    return policy, V
+
+if __name__ == "__main__":
+    env = gym.make('FrozenLake-v1')
+    policy, V = value_iteration(env)
+    print("Optimal Policy:")
+    print(policy)
+    print("Optimal Value Function:")
+    print(V)
+"""
+    return code
+
+def q_learning_heh():
+
+    code = """
+            import gym
+            import numpy as np
+
+            # Create FrozenLake environment
+            env = gym.make("FrozenLake-v1")
+
+            # Initialize Q-table
+            num_states = env.observation_space.n
+            num_actions = env.action_space.n
+            Q = np.zeros((num_states, num_actions))
+
+            # Q-learning parameters
+            alpha = 0.8  # Learning rate
+            gamma = 0.95  # Discount factor
+            epsilon = 0.1  # Exploration rate
+
+            # Q-learning algorithm
+            num_episodes = 10000
+            for episode in range(num_episodes):
+                state = env.reset()
+                done = False
+                while not done:
+                    # Choose action
+                    if np.random.uniform(0, 1) < epsilon:
+                        action = env.action_space.sample()  # Explore
+                    else:
+                        action = np.argmax(Q[state])  # Exploit
+
+                    # Take action
+                    next_state, reward, done, _ = env.step(action)
+
+                    # Update Q-table
+                    Q[state, action] += alpha * (reward + gamma * np.max(Q[next_state]) - Q[state, action])
+
+                    state = next_state
+
+            # Print the Q-table
+            print("Q-table:")
+            print(Q)
+
+            # Test the trained agent
+            num_test_episodes = 10
+            total_rewards = 0
+            for _ in range(num_test_episodes):
+                state = env.reset()
+                done = False
+                while not done:
+                    action = np.argmax(Q[state])
+                    next_state, reward, done, _ = env.step(action)
+                    total_rewards += reward
+                    state = next_state
+
+            avg_reward = total_rewards / num_test_episodes
+            print(f"Average reward over {num_test_episodes} test episodes: {avg_reward}")
+"""
+    return code
+
+def sarsa_heh():
+
+    code = """
+import numpy as np
+import gym
+
+# SARSA function approximation
+def sarsa(env, num_episodes, alpha, gamma, epsilon):
+    # Initialize Q table arbitrarily
+    Q = np.zeros((env.observation_space.n, env.action_space.n))
+    
+    # SARSA algorithm loop
+    for episode in range(num_episodes):
+        state = env.reset()
+        action = epsilon_greedy_policy(Q, state, epsilon)
+        
+        while True:
+            # Take action and observe next state and reward
+            next_state, reward, done, _ = env.step(action)
+            next_action = epsilon_greedy_policy(Q, next_state, epsilon)
+            
+            # Update Q-value
+            td_target = reward + gamma * Q[next_state][next_action]
+            td_error = td_target - Q[state][action]
+            Q[state][action] += alpha * td_error
+            
+            # Move to the next state and action
+            state = next_state
+            action = next_action
+            
+            if done:
+                break
+    
+    return Q
+
+# Epsilon-greedy policy
+def epsilon_greedy_policy(Q, state, epsilon):
+    if np.random.rand() < epsilon:
+        return env.action_space.sample()  # Exploration: choose random action
+    else:
+        return np.argmax(Q[state])  # Exploitation: choose action with highest Q-value
+
+# Main code
+if __name__ == "__main__":
+    # Create the environment
+    env = gym.make('Taxi-v3')
+    
+    # Set hyperparameters
+    num_episodes = 1000
+    alpha = 0.1
+    gamma = 0.99
+    epsilon = 0.1
+    
+    # Run SARSA algorithm
+    Q_values = sarsa(env, num_episodes, alpha, gamma, epsilon)
+    
+    # Print the learned Q-values
+    print("Learned Q-values:")
+    print(Q_values)
+"""
+    return code
+
+def monte_carlo_heh():
+
+    code = """
+import gym
+import numpy as np
+from collections import defaultdict
+
+def generate_episode(env, policy):
+    episode = []
+    state = env.reset()
+    while True:
+        player_sum, dealer_card, usable_ace = state
+        action = np.random.choice(len(policy[player_sum]))
+        next_state, reward, done, _ = env.step(action)
+        episode.append((state, action, reward))
+        if done:
+            break
+        state = next_state
+    return episode
+
+
+def monte_carlo_policy_evaluation(env, policy, num_episodes=100, gamma=1.0):
+    returns_sum = defaultdict(float)
+    returns_count = defaultdict(float)
+    V = defaultdict(float)
+
+    for _ in range(num_episodes):
+        episode = generate_episode(env, policy)
+        G = 0
+        for t in reversed(range(len(episode))):
+            state, action, reward = episode[t]
+            G = gamma * G + reward
+            if (state, action) not in [(e[0], e[1]) for e in episode[:t]]:
+                returns_sum[(state, action)] += G
+                returns_count[(state, action)] += 1
+                V[state] = returns_sum[(state, action)] / returns_count[(state, action)]
+
+    return V
+
+if __name__ == "__main__":
+    env = gym.make('Blackjack-v1')
+    policy = {i: [0.5, 0.5] for i in range(22)}  # Random policy
+    V = monte_carlo_policy_evaluation(env, policy, num_episodes=100, gamma=1.0)
+    print("Value Function:")
+    for state in sorted(V.keys()):
+      print(state, V[state])
+
+"""
     return code
```

### Comparing `spooling-0.0.3/spooling.egg-info/PKG-INFO` & `spooling-0.0.4/spooling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spooling
-Version: 0.0.3
+Version: 0.0.4
 Summary: rl experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spooling-0.0.3/spooling.egg-info/SOURCES.txt` & `spooling-0.0.4/spooling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

