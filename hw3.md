В качестве ДЗ изучить приложенный [файл](https://gbcdn.mrgcdn.ru/uploads/asset/4704179/attachment/8030f3621751282a7d05afc35133689b.cs)
* и описать блок-схему метода 4
// 4. метод, формирующий новый массив на основе имеющегося
int[] Solution(int[] collectionElements, int evenCounts)
  // 1 2 3 4 5 6 7 8 9 0 collectionElements
  // 2 0 0 0 0 items

{

  int[] items = new int[evenCounts];

  int length = collectionElements.Length;

  int position = 0;

  int indexInItems = 0;
  
  while (position < length)

  {

    if (collectionElements[position] % 2 == 0)
    {
      items[indexInItems] = collectionElements[position];
      indexInItems++;
    }
    position++;
  }
  return items;
}

[Блок-схема](Method4.png)


* попробовать объяснить почему метод PrintBad уступает методу PrintGood?
