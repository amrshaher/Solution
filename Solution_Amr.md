class Solution {

	public int solution(int k, int[] A) 
	{
		int count = 0;
		for (int p = 0; p < A.length; p++) 
		{
			for (int q = p; q < A.length; q++) 
			{
				if (((Math.max(A[p], A[q])) - (Math.min(A[p], A[q]))) <= k)
					 count++;				
			}
		}
		
		return count;
}
}
