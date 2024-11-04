```python
def matmul(left, right, output):
	B, M, K = left.shape
	_, N = right.shape

	for b in range(B):
		for m in range(M):
			for k in range(K):
				for n in range(N):
					output[b, m, n] += input[b, m, k] * output[k, n]
	# B M K N 任意调换顺序不影响结果

  
  

def add(output, bias):
	B, M, N = output.shape

	for b in range(B):
		for m in range(M):
			for n in range(n):
				output[b, m, n] += bias[n]

  
  

def matmul_add(left, right, bias, output):
	B, M, K = left.shape
	_, N = right.shape

	for b in range(B):
		for m in range(M):
			for n in range(N):
				output[b, m, n] = bias[n]
				for k in range(K):
					output[b, m, n] += input[b, m, k] * output[k, n]
```