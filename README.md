function sortOddNumbers(arr) {
    const oddNumbers = arr.filter(x => x % 2 !== 0).sort((a, b) => a - b);
    let oddIndex = 0;
    return arr.map(x => x % 2 !== 0 ? oddNumbers[oddIndex++] : x);
  }
  const arrays = [
    [7, 1],
    [5, 8, 6, 3, 4],
    [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
  ];
  arrays.forEach(arr => console.log(sortOddNumbers(arr)));
