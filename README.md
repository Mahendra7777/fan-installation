# fan-installation

n = int(input("Enter number of fans"));
v = int(input("Enter number of dependencies"));
adj = [for v in range (n)];
for i in range (0,d):
  u = int(input()); #Enter input between 0 and n-1
  v = int(input()); #Enter input between 0 and n-1
  adj[u].append(v);
 
vis = [0]*n;
stack = [];

def dfs(node):
  vis[node] = 1;
  for i in range (0,len(adj[node])):
   if vis[adj[node][i]] == 0:
   dfs(adj[node][i]);
  
 stack.append(node);
 
 for i in range(0,n):
  if vis[i] == 0:
    dfs(i)
 
while stack:
  print(stack.pop());
