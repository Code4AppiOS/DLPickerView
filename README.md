# DLPickerView
##一种支持单列数据选择，多列数据选择，plist读取数据选择的多功能数据选择器，只需改变选择器NSArray数据源即可！
###主要功能:
![Image text](https://raw.githubusercontent.com/coder-zwz/DLPickerView/master/screenshots/Simulator Screen Shot 2016年11月18日 上午10.27.58.png)
###多列数组数据源:
![Image text](https://raw.githubusercontent.com/coder-zwz/DLPickerView/master/screenshots/Simulator Screen Shot 2016年11月18日 上午10.27.58.png)
####多列数组数据源代码生成
      DLPickerView *pickerView = [[DLPickerView alloc] initWithDataSource:@[@[@"Bei Jing",@"Shang Hai"], @[@"Li Lei",@"Han Meimei"]]
                                                       withSelectedItem:[sender.titleLabel.text componentsSeparatedByString:OwnerSeparator]
                                                      withSelectedBlock:^(id selectedItem) {
                                                          [sender setTitle:[selectedItem componentsJoinedByString:OwnerSeparator] forState:UIControlStateNormal];
                                                      }
                                ];
    
    [pickerView show];


