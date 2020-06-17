# Slate

```c++
#include "FileTestStyle.h"



//#define ADD Initialize();#define 替换
//#号开头的都是预编译代码

TSharedPtr<FSlateStyleSet>FFileTestStyle::StyleInstance = NULL;

TSharedRef<FSlateStyleSet> FFileTestStyle::Create()
{
 TSharedRef<FSlateStyleSet>Style = MakeShareable(new FSlateStyleSet(GetStyleSetName()));
 Style->SetContentRoot(IPluginManager::Get().FindPlugin("FileTset")->GetBaseDir() / TEXT("Resoures"));//把style设置到Resoures根目录里
 Style->Set("FileTest.PluginAction", new FSlateImageBrush(Style->RootToContentDir(TEXT("Icon128.png")),FVector2D(40.0f,40.0f)));
 return Style;
}

void FFileTestStyle::ReloadTextures()
{
 if (FSlateApplication::IsInitialized()) {
  FSlateApplication::Get().GetRenderer()->ReloadTextureResources();

 }
}

const ISlateStyle& FFileTestStyle::Get()
{
 return*StyleInstance;
}

void FFileTestStyle::Initialize()
{
 if (!StyleInstance.IsValid()) 
 {
 StyleInstance = Create();
 FSlateStyleRegistry::UnRegisterSlateStyle(*StyleInstance);
 }
}

void FFileTestStyle::Shutdown()
{
 FSlateStyleRegistry::UnRegisterSlateStyle(*StyleInstance);
 StyleInstance.Reset();
}

FName FFileTestStyle::GetStyleSetName()
{
 //基础写法
 //return FName(TEXT("FileTestStyle"));
 static FName StyleSetName(TEXT("FileTestStyle"));
 return StyleSetName;
}
```

