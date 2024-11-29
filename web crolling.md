#직접 해보면서 배운것


dictionary 
```
person = {
    "name": "John",
    "age": 30,
    "city": "New York"}
print(person["name"])  # Output: John
출처: https://easyitwanner.tistory.com/270 [IT 시작해보기:티스토리]
```
{}이걸로 묶고 []이걸로 출력
```
product_data['review']  = review_tags.text.strip() 
```

이미지 주소 파싱하는거는 일반적인 텍스트 파싱하는거랑 왜 다른지.

텍스트만 파싱
```
text_tags = text_tags.text.strip()
```
이미지 주소 파싱
```
img_url = img_url['src'].strip()
```
src 속성은 이미지의 URL을 포함 BeautifulSoup 객체에서 속성에 접근하려면 딕셔너리 형태로 접근해야함.
