# Xamarin ListView Customizing it's ViewCell (cell)
[View Cell](https://developer.xamarin.com/guides/xamarin-forms/application-fundamentals/custom-renderer/viewcell/)

# ListView.HasUnevenRows
리스트뷰에 들어가는 아이템(Cell)들의 높이가 고정되지 않도록 설정해주는 속성
이 속성의 값이 True일 경우, 아이템들은 높이가 서로 다르게 설정될 수 있다.

# MVVM
Model-View-ViewModel
ViewModel은 VO 개념.. 뷰에 표시될 데이터를 저장하는 개체이다.<br />
View는 ViewModel을 뷰에 표시해주기 위해 데이터 바인딩을 해주는 녀석이다.<br />
Model은 컬렉션을 저장하고... 이 컬렉션을 View의 리스트 ItemsSource와 연동해주는 녀석인가..?

# WidthRequest, HeightRequest
뷰의 넓이와 높이가 얼마가 되어야 하는지를 결정하는 속성

# 자마린에서의 크기 값
iOS, Android에서는 160이 1인치(2.54cm), UWP(Windows Phone)에서는 240이 1인치가 된다.<br />
iOS, Android에서는 64가 1cm, UWP에선 96이 1cm..<br />
코드를 통해서만 플랫폼 별로 독립적인 크기를 줄 수 있는지..?<br />
아니면 XAML를 통해서 플랫폼 별로 독립적인 크기를 줄 수 있는지...? - 해결해보자

# 데이터 바인딩
StaticResource - App.xaml에서 정의된 Resource를 key로 접근할 수 있다.
{StaticResource key} 형태로 사용 가능..

만약, 바인딩한 데이터에 가공이 필요하다면 컨버터를 사용한다.<br />
{Binding 속성이름, Converter={StaticResource 컨버터 키 값}[, ConverterParameter='필요하다면 매개변수'}

EZ
