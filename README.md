local function CreateInstance(cls,props)
    local inst = Instance.new(cls)
    for i,v in pairs(props) do
        inst[i] = v
    end
    return inst
    end
    local Enabled = false
    inv = false
    usestorage = false	
    local NovaV8 = CreateInstance('ScreenGui',{DisplayOrder=0,Enabled=true,ResetOnSpawn=true,Name='NovaV8', Parent=game.CoreGui})
    local openedgui = CreateInstance('ImageLabel',{Image='rbxassetid://2851926732',ImageColor3=Color3.new(0.156863, 0.156863, 0.156863),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0.079999998211861,ScaleType=Enum.ScaleType.Slice,SliceCenter=Rect.new(12, 12, 12, 12),Active=true,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=true,Draggable=true,Position=UDim2.new(0.517, 0, -1, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 383, 0, 194),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='openedgui',Parent = NovaV8})
    local btnItalyGUI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size14,Text='Italy',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.580392, 0.764706, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.468823373, 0, 0.0686843693, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 74, 0, 25),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnItalyGUI',Parent = openedgui})
    local btnMoriohGUI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size14,Text='Morioh',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.262745, 0.47451, 0.67451),BackgroundTransparency=1,BorderColor3=Color3.new(1, 1, 1),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.184387445, 0, 0.0686521977, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 75, 0, 25),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnMoriohGUI',Parent = openedgui})
    local btnSpecialGui = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size14,Text='Special',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.576471, 0.619608, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.75741601, 0, 0.0686521977, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 76, 0, 25),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnSpecialGui',Parent = openedgui})
    local closegui = CreateInstance('ImageButton',{Image='rbxassetid://3494886164',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.965316355, 0, 0.0659565106, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 23, 0, 24),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='closegui',Parent = openedgui})
    local line = CreateInstance('Frame',{Style=Enum.FrameStyle.Custom,Active=false,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.999992, 0.505471, 6.73556e-05),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(-0.0883179903, 0, 0.125935122, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 66, 0, 2),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name = 'line',Parent = openedgui})
    local MoriohGui = CreateInstance('ScrollingFrame',{BottomImage='rbxasset://textures/ui/Scroll/scroll-bottom.png',CanvasPosition=Vector2.new(0, 0),CanvasSize=UDim2.new(0, 0, 0.899999976, 0),MidImage='rbxasset://textures/ui/Scroll/scroll-middle.png',ScrollBarThickness=12,ScrollingEnabled=true,TopImage='rbxasset://textures/ui/Scroll/scroll-top.png',Active=false,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.156863, 0.156863, 0.156863),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.499000013, 0, 3, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 383, 0, 152),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='MoriohGui',Parent = openedgui})
    local btnmoney = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Money Farm',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 11),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnmoney',Parent = MoriohGui})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584120281',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnmoney})
    local btnlevel = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Level Farm',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 11),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnlevel',Parent = MoriohGui})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584020980',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnlevel})
    local btnfarmitem = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Items Farm',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 122),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnfarmitem',Parent = MoriohGui})
    local ImageLabel = CreateInstance('ImageLabel',{Image='rbxassetid://4498590361',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnfarmitem})
    local btnnpc = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Npc TP',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 65),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnnpc',Parent = MoriohGui})
    local ImageLabel = CreateInstance('ImageLabel',{Image='rbxassetid://4498590361',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnnpc})
    local btnOpenStandGUIm = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Stand Farm',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 122),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnOpenStandGUIm',Parent = MoriohGui})
    local ImageLabel = CreateInstance('ImageLabel',{Image='rbxassetid://4498590361',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnOpenStandGUIm})
    local btnworthm = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Worth Farm',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, -1, 0, 65),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnworthm',Parent = MoriohGui})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584022155',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnworthm})
    local ItalyGUI = CreateInstance('ScrollingFrame',{BottomImage='rbxasset://textures/ui/Scroll/scroll-bottom.png',CanvasPosition=Vector2.new(0, 0),CanvasSize=UDim2.new(0, 0, 0.899999976, 0),MidImage='rbxasset://textures/ui/Scroll/scroll-middle.png',ScrollBarThickness=12,ScrollingEnabled=true,TopImage='rbxasset://textures/ui/Scroll/scroll-top.png',Active=false,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.156863, 0.156863, 0.156863),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.499000013, 0, 3, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 383, 0, 152),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ItalyGUI',Parent = openedgui})
    local btnmoneyI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Money Farm',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 11),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnmoneyI',Parent = ItalyGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584120281',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnmoneyI})
    local btnlevelI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Level Farm',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 11),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnlevelI',Parent = ItalyGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584020980',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnlevelI})
    local btnFarmWorth = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Worth Farm',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 65),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnFarmWorth',Parent = ItalyGUI})
    local imagefw = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584022155',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='imagefw',Parent = btnFarmWorth})
    local btnfarmitemI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Items Farm',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 119),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnfarmitemI',Parent = ItalyGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='rbxassetid://4498590361',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnfarmitemI})
    local btnOpenStandGUI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Stand Farm',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 65),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnOpenStandGUI',Parent = ItalyGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='rbxassetid://4498590361',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnOpenStandGUI})
    local SpecialGUI = CreateInstance('ScrollingFrame',{BottomImage='rbxasset://textures/ui/Scroll/scroll-bottom.png',CanvasPosition=Vector2.new(0, 0),CanvasSize=UDim2.new(0, 0, 2, 0),MidImage='rbxasset://textures/ui/Scroll/scroll-middle.png',ScrollBarThickness=12,ScrollingEnabled=true,TopImage='rbxasset://textures/ui/Scroll/scroll-top.png',Active=false,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.156863, 0.156863, 0.156863),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.499000013, 0, 3, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 383, 0, 155),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='SpecialGUI',Parent = openedgui})
    local btnfusion = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='           Temporary Fusion',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 11),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnfusion',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='rbxassetid://4498590361',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.0741340742, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnfusion})
    local btnTimeStop = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Anti-TimeStop',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 11),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnTimeStop',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584021755',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnTimeStop})
    local btnalert = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Boss Alert',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 117),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnalert',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584019678',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnalert})
    local btnkillgui = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Kill Boss',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 117),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnkillgui',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584349325',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnkillgui})
    local btntpitaly = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          TP Italy',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 65),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btntpitaly',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584020683',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btntpitaly})
    local btndupe = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Dupe Function',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 175),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btndupe',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584353841',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btndupe})
    local btnstatschanger = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Stats changer',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 287),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnstatschanger',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584021412',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnstatschanger})
    local btnstandstorage = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Stand Storage',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 65),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnstandstorage',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584021904',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnstandstorage})
    local btnjotaro = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Jotaro Auto-Quest',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 175),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnjotaro',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584384541',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnjotaro})
    local btnesp = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Esp',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 287),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnesp',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4588047111',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnesp})
    local btninvisible = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Invisible',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 341),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btninvisible',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584020284',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btninvisible})
    local btnshop = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Shop',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 341),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnshop',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584021263',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnshop})
    local btnrohan = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Rohan Auto-Quest',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 231),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnrohan',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=5705953462',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.0853072554, -4, 0.0787234083, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnrohan})
    local btnboom = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='         Music',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 231),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='btnboom',Parent = SpecialGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=5721695989',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = btnboom})
    local ItensGUI = CreateInstance('ScrollingFrame',{BottomImage='rbxasset://textures/ui/Scroll/scroll-bottom.png',CanvasPosition=Vector2.new(0, 0),CanvasSize=UDim2.new(0, 0, 2, 0),MidImage='rbxasset://textures/ui/Scroll/scroll-middle.png',ScrollBarThickness=12,ScrollingEnabled=true,TopImage='rbxasset://textures/ui/Scroll/scroll-top.png',Active=false,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.156863, 0.156863, 0.156863),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.499000013, 0, 3, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 383, 0, 152),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ItensGUI',Parent = openedgui})
    local getRokaka = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Rokaka Fruit',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 34),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getRokaka',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584021601',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getRokaka})
    local getArrow = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Arrow',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 34),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getArrow',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584019548',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getArrow})
    local getMask = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Vampire Mask',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 140),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getMask',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584022027',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getMask})
    local getAja = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Red Stone Of Aja',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 88),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getAja',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584019353',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getAja})
    local getDiary = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Dio\'s Diary',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.380392, 0.407843, 0.207843),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 88),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getDiary',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4790257826',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getDiary})
    local getReqArrow = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Requiem Arrow',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.305882, 0.207843, 0.317647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 194),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getReqArrow',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584019548',ImageColor3=Color3.new(0.403922, 0.694118, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getReqArrow})
    local getDisk = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Disk',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.305882, 0.207843, 0.317647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 191, 0, 194),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getDisk',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=5705976440',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getDisk})
    local getSRokaka = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Stone Rokaka',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 188, 0, 140),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getSRokaka',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584021601',ImageColor3=Color3.new(0.631373, 0.631373, 0.631373),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getSRokaka})
    local text = CreateInstance('TextLabel',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size14,Text='Auto-Store',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.384203643, 0, 0.0556032211, 0),Rotation=0,Selectable=false,Size=UDim2.new(0.224807143, 0, 0.114306413, 0),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='text',Parent = ItensGUI})
    local Frame = CreateInstance('ImageLabel',{Image='rbxassetid://2851926732',ImageColor3=Color3.new(0.113725, 0.113725, 0.113725),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Slice,SliceCenter=Rect.new(12, 12, 12, 12),Active=false,AnchorPoint=Vector2.new(0, 0.5),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1.0883857, 0, 0.449365973, 0),Rotation=0,Selectable=false,Size=UDim2.new(0.504746974, 0, 0.391045868, 0),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='Frame',Parent = text})
    local storemorioh = CreateInstance('TextButton',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size14,Text='',TextColor3=Color3.new(0, 0, 0),TextScaled=true,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.00392157, 0.756863, 0.254902),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(0.34526816, 0, 0.999999642, 0),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='storemorioh',Parent = Frame})
    local Textcolorstorem = CreateInstance('ImageLabel',{Image='rbxassetid://2851926732',ImageColor3=Color3.new(0.635294, 0, 0),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Slice,SliceCenter=Rect.new(12, 12, 12, 12),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=false,Size=UDim2.new(1.24948788, 0, 1, 0),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='Textcolorstorem',Parent = storemorioh})
    local TextLabel = CreateInstance('TextLabel',{Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,Text='Fireclickdetector Needed',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.271540463, 0, 0.65558517, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 173, 0, 14),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='TextLabel',Parent = ItensGUI})
    local getwrench = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Wrench',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 279),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getwrench',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=5720522631',ImageColor3=Color3.new(0.631373, 0.631373, 0.631373),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getwrench})
    local getmoneybag = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Money Bag',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 279),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getmoneybag',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584120281',ImageColor3=Color3.new(0.631373, 0.631373, 0.631373),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getmoneybag})
    local getdiobone = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Dio Bone(Worth)',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=15,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 187, 0, 335),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getdiobone',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=5706028002',ImageColor3=Color3.new(0.631373, 0.631373, 0.631373),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getdiobone})
    local getdiodiary = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Dio Diary(Worth)',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=15,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 0, 0, 335),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getdiodiary',Parent = ItensGUI})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4790257826',ImageColor3=Color3.new(0.631373, 0.631373, 0.631373),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getdiodiary})
    local StatsChanger = CreateInstance('ScrollingFrame',{BottomImage='rbxasset://textures/ui/Scroll/scroll-bottom.png',CanvasPosition=Vector2.new(0, 0),CanvasSize=UDim2.new(0, 0, 0.899999976, 0),MidImage='rbxasset://textures/ui/Scroll/scroll-middle.png',ScrollBarThickness=12,ScrollingEnabled=true,TopImage='rbxasset://textures/ui/Scroll/scroll-top.png',Active=false,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.156863, 0.156863, 0.156863),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.499000013, 0, 3, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 383, 0, 154),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='StatsChanger',Parent = openedgui})
    local TextLabel = CreateInstance('TextLabel',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size14,Text='Stats Changer',TextColor3=Color3.new(1, 1, 1),TextScaled=true,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.33044219, 0, 0.0246093478, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 129, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='TextLabel',Parent = StatsChanger})
    local TextLabel = CreateInstance('TextLabel',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size14,Text='Normal',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.0876223296, 0, 0.143587783, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 129, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='TextLabel',Parent = StatsChanger})
    local TextLabel = CreateInstance('TextLabel',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size14,Text='Advanced',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.565429151, 0, 0.143587783, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 129, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='TextLabel',Parent = StatsChanger})
    local powerv = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='',TextColor3=Color3.new(0, 0, 0), PlaceholderText='', PlaceholderColor3=Color3.new(0.7, 0.7, 0.7),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.272196174, 0, 0.255876958, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 77, 0, 24),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='powerv',Parent = StatsChanger})
    local powerc = CreateInstance('TextButton',{Font=Enum.Font.SourceSansBold,FontSize=Enum.FontSize.Size18,Text='Power',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.0784314, 0.0784314, 0.0784314),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.0313315913, 0, 0.256151229, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 80, 0, 23),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='powerc',Parent = StatsChanger})
    local endurancev = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='1.2004',TextColor3=Color3.new(0, 0, 0), PlaceholderText='', PlaceholderColor3=Color3.new(0.7, 0.7, 0.7),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.272196174, 0, 0.506972253, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 77, 0, 24),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='endurancev',Parent = StatsChanger})
    local endurancec = CreateInstance('TextButton',{Font=Enum.Font.SourceSansBold,FontSize=Enum.FontSize.Size18,Text='Endurance',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.0784314, 0.0784314, 0.0784314),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.0313315913, 0, 0.507246315, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 80, 0, 23),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='endurancec',Parent = StatsChanger})
    local specialv = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='1.2998',TextColor3=Color3.new(0, 0, 0), PlaceholderText='', PlaceholderColor3=Color3.new(0.7, 0.7, 0.7),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.272196174, 0, 0.744494438, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 77, 0, 24),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='specialv',Parent = StatsChanger})
    local specialc = CreateInstance('TextButton',{Font=Enum.Font.SourceSansBold,FontSize=Enum.FontSize.Size18,Text='Special',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.0784314, 0.0784314, 0.0784314),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.0313315913, 0, 0.744768679, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 80, 0, 23),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='specialc',Parent = StatsChanger})
    local speedv = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='',TextColor3=Color3.new(0, 0, 0), PlaceholderText='', PlaceholderColor3=Color3.new(0.7, 0.7, 0.7),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.734060168, 0, 0.744494438, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 77, 0, 24),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='speedv',Parent = StatsChanger})
    local potencyv = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='',TextColor3=Color3.new(0, 0, 0), PlaceholderText='', PlaceholderColor3=Color3.new(0.7, 0.7, 0.7),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.734060168, 0, 0.255876958, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 77, 0, 24),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='potencyv',Parent = StatsChanger})
    local resiliencev = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='1.15',TextColor3=Color3.new(0, 0, 0), PlaceholderText='', PlaceholderColor3=Color3.new(0.7, 0.7, 0.7),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.734060168, 0, 0.506972253, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 77, 0, 24),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='resiliencev',Parent = StatsChanger})
    local potencyc = CreateInstance('TextButton',{Font=Enum.Font.SourceSansBold,FontSize=Enum.FontSize.Size18,Text='Potency',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.0784314, 0.0784314, 0.0784314),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.493195683, 0, 0.256151229, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 80, 0, 23),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='potencyc',Parent = StatsChanger})
    local resiliencec = CreateInstance('TextButton',{Font=Enum.Font.SourceSansBold,FontSize=Enum.FontSize.Size18,Text='Resilience',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.0784314, 0.0784314, 0.0784314),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.493195683, 0, 0.507246315, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 80, 0, 23),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='resiliencec',Parent = StatsChanger})
    local speedc = CreateInstance('TextButton',{Font=Enum.Font.SourceSansBold,FontSize=Enum.FontSize.Size18,Text='Speed',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.0784314, 0.0784314, 0.0784314),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.493195683, 0, 0.744768679, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 80, 0, 23),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='speedc',Parent = StatsChanger})
    local logobackground = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4581878998',ImageColor3=Color3.new(0, 0, 0),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0.89999997615814,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.315926909, 0, 0.216494843, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 141, 0, 141),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='logobackground',Parent = openedgui})
    local npcs = CreateInstance('ScrollingFrame',{BottomImage='rbxasset://textures/ui/Scroll/scroll-bottom.png',CanvasPosition=Vector2.new(0, 0),CanvasSize=UDim2.new(0, 0, 0.899999976, 0),MidImage='rbxasset://textures/ui/Scroll/scroll-middle.png',ScrollBarThickness=12,ScrollingEnabled=true,TopImage='rbxasset://textures/ui/Scroll/scroll-top.png',Active=false,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.156863, 0.156863, 0.156863),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.499000013, 0, 3, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 383, 0, 154),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='npcs',Parent = openedgui})
    local TextLabel = CreateInstance('TextLabel',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size14,Text='Npc Chooser',TextColor3=Color3.new(1, 1, 1),TextScaled=true,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.33044219, 0, 0.0246093478, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 129, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='TextLabel',Parent = npcs})
    local gyrotp = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='Gyro',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.314020932, 0, 0.206623524, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 140, 0, 24),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='gyrotp',Parent = npcs})
    local caesartp = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='Caesar',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.314020932, 0, 0.445680887, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 140, 0, 24),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='caesartp',Parent = npcs})
    local zeppelitp = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='Zeppeli',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.314020932, 0, 0.703611135, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 140, 0, 24),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='zeppelitp',Parent = npcs})
    local ItensGUIi = CreateInstance('ScrollingFrame',{BottomImage='rbxasset://textures/ui/Scroll/scroll-bottom.png',CanvasPosition=Vector2.new(0, 0),CanvasSize=UDim2.new(0, 0, 1.79999995, 0),MidImage='rbxasset://textures/ui/Scroll/scroll-middle.png',ScrollBarThickness=12,ScrollingEnabled=true,TopImage='rbxasset://textures/ui/Scroll/scroll-top.png',Active=false,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(0.156863, 0.156863, 0.156863),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0.499000013, 0, 3, 0),Rotation=0,Selectable=true,Size=UDim2.new(0, 383, 0, 152),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ItensGUIi',Parent = openedgui})
    local text = CreateInstance('TextLabel',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size14,Text='Auto-Store',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(0.5, 0.5),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.384203643, 0, 0.0556032211, 0),Rotation=0,Selectable=false,Size=UDim2.new(0.224807143, 0, 0.114306413, 0),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='text',Parent = ItensGUIi})
    local Frame = CreateInstance('ImageLabel',{Image='rbxassetid://2851926732',ImageColor3=Color3.new(0.113725, 0.113725, 0.113725),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Slice,SliceCenter=Rect.new(12, 12, 12, 12),Active=false,AnchorPoint=Vector2.new(0, 0.5),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1.0883857, 0, 0.449365973, 0),Rotation=0,Selectable=false,Size=UDim2.new(0.504746974, 0, 0.391045868, 0),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='Frame',Parent = text})
    local storeitaly = CreateInstance('TextButton',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size14,Text='',TextColor3=Color3.new(0, 0, 0),TextScaled=true,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.00392157, 0.756863, 0.254902),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(0.34526816, 0, 0.999999642, 0),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='storeitaly',Parent = Frame})
    local Textcolorstorei = CreateInstance('ImageLabel',{Image='rbxassetid://2851926732',ImageColor3=Color3.new(0.635294, 0, 0),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Slice,SliceCenter=Rect.new(12, 12, 12, 12),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=false,Size=UDim2.new(1.24948788, 0, 1, 0),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='Textcolorstorei',Parent = storeitaly})
    local TextLabel = CreateInstance('TextLabel',{Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,Text='Fireclickdetector Needed',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.282000005, 0, 0.579999983, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 173, 0, 14),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='TextLabel',Parent = ItensGUIi})
    local getmoneybagI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Money Bag',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 4, 0, 227),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getmoneybagI',Parent = ItensGUIi})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584120281',ImageColor3=Color3.new(0.631373, 0.631373, 0.631373),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getmoneybagI})
    local getdioboneI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Dio Bone(Worth)',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=15,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 4, 0, 288),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getdioboneI',Parent = ItensGUIi})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=5706028002',ImageColor3=Color3.new(0.631373, 0.631373, 0.631373),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getdioboneI})
    local getdiodiaryI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Dio Diary(Worth)',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=15,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 196, 0, 227),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getdiodiaryI',Parent = ItensGUIi})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4790257826',ImageColor3=Color3.new(0.631373, 0.631373, 0.631373),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getdiodiaryI})
    local getAjaI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Red Stone Of Aja',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=true,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 191, 0, 86),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getAjaI',Parent = ItensGUIi})
    local imagerai = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584019353',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='imagerai',Parent = getAjaI})
    local getAjaMaskI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Aja Mask',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 4, 0, 32),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getAjaMaskI',Parent = ItensGUIi})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584022027',ImageColor3=Color3.new(1, 0.360784, 0.372549),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getAjaMaskI})
    local getCorpse = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Corpse Part',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 191, 0, 32),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getCorpse',Parent = ItensGUIi})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584019826',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getCorpse})
    local getDiskI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Disk',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.317647, 0.2, 0.239216),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 4, 0, 145),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getDiskI',Parent = ItensGUIi})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=5705976440',ImageColor3=Color3.new(1, 1, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getDiskI})
    local getReqArrowI = CreateInstance('TextButton',{Font=Enum.Font.GothamSemibold,FontSize=Enum.FontSize.Size18,Text='          Requiem Arrow',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.117647, 0.117647, 0.117647),BackgroundTransparency=0,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=0,ClipsDescendants=true,Draggable=false,Position=UDim2.new(0, 4, 0, 86),Rotation=0,Selectable=true,Size=UDim2.new(0, 179, 0, 47),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='getReqArrowI',Parent = ItensGUIi})
    local ImageLabel = CreateInstance('ImageLabel',{Image='http://www.roblox.com/asset/?id=4584019548',ImageColor3=Color3.new(0.403922, 0.694118, 1),ImageRectOffset=Vector2.new(0, 0),ImageRectSize=Vector2.new(0, 0),ImageTransparency=0,ScaleType=Enum.ScaleType.Stretch,SliceCenter=Rect.new(0, 0, 0, 0),Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0.129999995, -4, 0.100000001, 2),Rotation=0,Selectable=false,Size=UDim2.new(0, 35, 0, 35),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ImageLabel',Parent = getReqArrowI})
    players = game.Players:GetChildren()
    --functions
    btn=btnMoriohGUI
    function touch()
        local ms = game.Players.LocalPlayer:GetMouse()
        local c = game.CoreGui.NovaV7m.b2.Sample:Clone()
        c.Parent = btn
        local x, y = (ms.X - c.AbsolutePosition.X), (ms.Y - c.AbsolutePosition.Y)
        c.Position = UDim2.new(0, x, 0, y)
        local len, size = 0.35, nil
        if btn.AbsoluteSize.X >= btn.AbsoluteSize.Y then
            size = (btn.AbsoluteSize.X * 1.5)
        else
            size = (btn.AbsoluteSize.Y * 1.5)
        end
        c:TweenSizeAndPosition(UDim2.new(0, size, 0, size), UDim2.new(0.5, (-size / 2), 0.5, (-size / 2)), 'Out', 'Quad', len, true, nil)
        for i = 1, 10 do
            c.ImageTransparency = c.ImageTransparency + 0.05
            wait(len / 12)
        end
        c:Destroy()
    end
    function notif(titl,tex,durat)
        game.StarterGui:SetCore("SendNotification",{Title = titl;Text = tex;Duration = durat;})
    end
    function FindStore(target)
        for i, v in next, game.Players.LocalPlayer:GetChildren() do
            if string.find(v.Name, target) then 
                if v.Value == "None" then
                    local str = string.match(v.Name,"%d+")
                    matable = {}
                    table.insert(matable,str)
                    game:GetService("ReplicatedStorage").Logic.storeitem:FireServer(0,tonumber(matable[1]))
                    game:GetService("ReplicatedStorage").Logic.storeitem:FireServer(1)
                end
            end
        end
    end
    function slots()
        if game.Players.LocalPlayer.HasBag.Value==false then
            FindStore("storeditem19")
            wait(1)
            FindStore("storeditem20")
            wait(1)
            FindStore("storeditem21")
        else
            FindStore("storeditem")
        end
    end
    function check(target)
        if usestorage==true then
            for i,v in next, game.Players.LocalPlayer.Character:GetChildren() do
                if v.Name== target then
                    slots()
                end
            end
            for i,v in next, game.Players.LocalPlayer.Backpack:GetChildren() do
                if v.Name== target then
                    v.Parent=game.Players.LocalPlayer.Character
                    slots()
                end
            end
        end
    end
    function itemget(target)
        local item = workspace:WaitForChild(target)
        if item then
            local player = game.Players.LocalPlayer.Character.HumanoidRootPart
            x = player.Position.X
            y = player.Position.Y
            z = player.Position.Z
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = item.Handle.CFrame
            wait(.5)
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(x,y,z)
            check(target)
        end
    end
    function npcget(target)
        local npc = workspace:WaitForChild(target)
        if npc then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace[target].ClickPart.CFrame 
        end
    end
    function entrar(target)
        target:TweenPosition(UDim2.new(0.499, 0, 0.53, 0))
    end
    function sair(target)
        target:TweenPosition(UDim2.new(0.499, 0, 3, 0))
    end
    --Open GUI / CLOSE
    openedgui:TweenPosition(UDim2.new(0.517, 0, 0.547, 0))
    game.Players.LocalPlayer:GetMouse().KeyDown:connect(function(menu)
        if (menu=="x") then
            Enabled = false
        end
    end)
    btnMoriohGUI.MouseButton1Click:Connect(function()
        btn=btnMoriohGUI
        touch();line:TweenPosition(UDim2.new(0.183, 0,0.126, 0));sair(SpecialGUI);sair(ItensGUI);sair(ItensGUIi);sair(StatsChanger);sair(ItalyGUI);sair(npcs);entrar(MoriohGui);logobackground.Visible=false;
    end)
    btnItalyGUI.MouseButton1Click:Connect(function()
        btn=btnItalyGUI
        touch();line:TweenPosition(UDim2.new(0.468, 0,0.126, 0));sair(SpecialGUI);sair(ItensGUI);sair(ItensGUIi);sair(StatsChanger);sair(MoriohGui);sair(npcs);entrar(ItalyGUI);logobackground.Visible=false;
    end)
    btnSpecialGui.MouseButton1Click:Connect(function()
        btn=btnSpecialGui;touch();sair(line);sair(ItalyGUI);sair(ItensGUI);sair(ItensGUIi);sair(StatsChanger);sair(MoriohGui);sair(npcs);entrar(SpecialGUI);logobackground.Visible=false;
    end)
    closegui.MouseButton1Click:Connect(function()
        btn=closegui
        touch();openedgui:TweenPosition(UDim2.new(0.517, 0, -1, 0));
    end)
    --Morioh
    btnlevel.MouseButton1Click:Connect(function()
        btn=btnlevel
        touch();Enabled = true;
        while Enabled == true do
            game:GetService("ReplicatedStorage").Logic.hitbox:InvokeServer(81,game.Players.LocalPlayer.Character.HumanoidRootPart,CFrame.new(nil,nil,nil),20000,game.Players.LocalPlayer.Character.Torso.voiceline,game:GetService("Workspace")["Ultimate Dummy"].Humanoid,false)
            game:GetService("ReplicatedStorage").Specials.healevent:FireServer(CFrame.new(nil, nil, nil),math.huge,game:GetService("Workspace")["Ultimate Dummy"]:WaitForChild("Humanoid"),game.Players.LocalPlayer.Character.Torso.voiceline,false)
        end
    end)
    btnmoney.MouseButton1Click:Connect(function()
        btn=btnmoney
        touch()
        Enabled = true
        for i,v in next, debug.getregistry() do
            if type(v) == "string" then
                for a,b in next, debug.getupvalues(v) do
                    if string.find(a, "cooled") or string.find(a, "cooled2") or string.find(a, "cooled3") or string.find(a, "cooled4") or string.find(a, "cooled5") or string.find(a, "cooledz") then
                        debug.setupvalue(v, a, true)
                    end
                end
            end
        end
        local function Kills()
            while Enabled == true do 
                for i,v in pairs(game.Workspace:GetChildren()) do
                    if v.Name == "Giant Dummy" or v.Name == "Metal Dummy" or v.Name == "Wood Dummy" or v.Name == "Ice Dummy" or v.Name == "Rock Dummy" then
                        game:GetService("ReplicatedStorage").Specials.healevent:FireServer(CFrame.new(nil, nil, nil),math.huge,v.Humanoid,game.Players.LocalPlayer.Character.Torso.voiceline,false)
                        game.ReplicatedStorage.Logic.hitbox:InvokeServer(99, game.Players.LocalPlayer.Character.Head, CFrame.new(nil, nil, nil), math.huge, game.Players.LocalPlayer.Character.Torso.voiceline, v.Humanoid, false, false, false)
                        if Enabled == false then break end
                    end
                end
            end
        end
        for i = 1, 130 do
            spawn(Kills)
	    wait(0.5)
        end
    end)
    btnfarmitem.MouseButton1Click:Connect(function()
        btn=btnfarmitem
        touch();sair(ItalyGUI);sair(MoriohGui);sair(SpecialGUI);entrar(ItensGUI)
    end)
    btnnpc.MouseButton1Click:Connect(function()
        btn=btnnpc
        touch();sair(MoriohGui);entrar(npcs)
    end)
    btnworthm.MouseButton1Click:Connect(function()
        btn=btnworthm
        touch()
        local function fastkill(humanoid)
            game.ReplicatedStorage.Specials.healevent:FireServer(CFrame.new(),math.huge, humanoid, workspace:FindFirstChildOfClass("Sound"), false)
            game.ReplicatedStorage.Logic.hitbox:InvokeServer(99, game.Players.LocalPlayer.Character.Head, CFrame.new(),math.huge, workspace:FindFirstChildOfClass("Sound"), humanoid, false, false, false)
        end
        local function worth()
            for i=0,7 do
                fastkill(workspace["Titan Dummy"].Humanoid)
            end
            wait(20)
            if game.Players.LocalPlayer.Worth.Value < 100 then
                fireclickdetector(workspace["Assault The Titans"].ClickPart.ClickDetector)
            end
        end
        if game.Players.LocalPlayer.Worth.Value < 100 then
            fireclickdetector(workspace["Assault The Titans"].ClickPart.ClickDetector)
        end
        local worh = game:GetService("Players").LocalPlayer:WaitForChild("GyroQuest13")
        if worh then
            while game.Players.LocalPlayer.Worth.Value < 100 do
                worth()
            end
        end
    end)
    btnOpenStandGUIm.MouseButton1Click:Connect(function()
        btn=btnOpenStandGUIm
        touch()
        local standcheckm = game.CoreGui:FindFirstChild("StandsFarm")
        if standcheckm then
            game.CoreGui.StandsFarm.StandsGUI:TweenPosition(UDim2.new(0.498945326, 0, 0.545793176, 0))
        else
            loadstring(game:HttpGet("https://raw.githubusercontent.com/yhuhuong2567/estu/main/README.md", true))()	
        end
    end)
    --NPC
    gyrotp.MouseButton1Click:Connect(function()
        btn=gyrotp
        touch();notif("Searching Gyro","When spawned automatically Tp to him",5);npcget("Gyro")
    end)
    caesartp.MouseButton1Click:Connect(function()
        btn=caesartp
        touch();notif("Searching Caesar","When spawned automatically Tp to him",5);npcget("Caesar")
    end)
    zeppelitp.MouseButton1Click:Connect(function()
        btn=zeppelitp
        touch();notif("Searching Zeppeli","When spawned automatically Tp to him",5);npcget("Zeppeli")
    end)
    --FarmItems(Morioh)
    getAja.MouseButton1Click:Connect(function()
        btn=getAja
        touch();notif("Searching RedAja","When spawned teleport it to you",5);itemget("RedAja")
    end)
    getArrow.MouseButton1Click:Connect(function()
        btn=getArrow
        touch();notif("Searching Arrow","When spawned teleport it to you",5);itemget("StandArrow")
    end)
    getRokaka.MouseButton1Click:Connect(function()
        btn=getRokaka
        touch();notif("Searching Rokaka","When spawned teleport it to you",5);itemget("RokakakaFruit")
    end)
    getMask.MouseButton1Click:Connect(function()
        btn=getMask
        touch();notif("Searching VampireMask","When spawned teleport it to you",5);itemget("VampireMask")
    end)
    getDiary.MouseButton1Click:Connect(function()
        btn=getDiary
        touch();notif("Searching Dio Diary","When spawned teleport it to you,remember you need kill Dio for spawn it",5);itemget("Dio's Diary")
    end)
    getDisk.MouseButton1Click:Connect(function()
        btn=getDisk
        touch();notif("Searching Disk","When spawned auto use it,remember you need kill Dio or Kira for spawn it",5)
        local item = workspace:WaitForChild("bossdisc")
        if item then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = item.CFrame
            wait(0.5)
            fireclickdetector(item.ClickDetector)
        end
    end)
    getReqArrow.MouseButton1Click:Connect(function()
        btn=getReqArrow
        touch();notif("Searching Requiem Arrow","When spawned teleport it to you,remember you need kill Kira for spawn it",5);itemget("RequiemArrow")
    end)
    getSRokaka.MouseButton1Click:Connect(function()
        btn=getSRokaka
        touch();notif("Searching Stone Rokaka","When spawned teleport it to you",5);itemget("StoneRokakakaFruit")
    end)
    getdiobone.MouseButton1Click:Connect(function()
        btn=getdiobone
        touch();notif("Searching Bone","When spawned auto use it",5)
        local item = workspace:WaitForChild("DioBone")
        if item then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = item.CFrame
            wait(0.5)
            fireclickdetector(item.ClickDetector)
        end
    end)
    getdiodiary.MouseButton1Click:Connect(function()
        btn=getdiodiary
        touch();notif("Searching Diary","When spawned auto use it",5)
        local item = workspace:WaitForChild("DioDiary")
        if item then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = item.CFrame
            wait(0.5)
            fireclickdetector(item.ClickDetector)
        end
    end)
    getmoneybag.MouseButton1Click:Connect(function()
        btn=getmoneybag
        touch();notif("Searching Money","When spawned auto use it",5)
        local item = workspace:WaitForChild("MoneyBag")
        if item then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = item.CFrame
            wait(0.5)
            fireclickdetector(item.ClickDetector)
        end
    end)
    getwrench.MouseButton1Click:Connect(function()
        btn=getmoneybag
        touch();notif("Searching Wrench","When spawned auto use it",5)
        local item = workspace:WaitForChild("Wrench")
        if item then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = item.CFrame
            wait(0.5)
            fireclickdetector(item.ClickDetector)
        end
    end)
    storemorioh.MouseButton1Click:Connect(function()
        btn=storemorioh
        touch()
        if usestorage==false then
            usestorage=true
            Textcolorstorem.ImageColor3 = Color3.fromRGB(1, 193, 65)
            storemorioh:TweenPosition(UDim2.new(0.501, 0,0, 0),"Out","Linear",0.1,false,nil)
        else
            usestorage=false
            Textcolorstorem.ImageColor3 = Color3.fromRGB(162, 0, 0)
            storemorioh:TweenPosition(UDim2.new(0, 0,0, 0),"Out","Linear",0.1,false,nil)
        end
    end)
    --Italy
    btnlevelI.MouseButton1Click:Connect(function()
        btn=btnlevelI
        touch()
        Enabled = true
        while Enabled == true do
            game:GetService("ReplicatedStorage").Logic.hitbox:InvokeServer(1,nil,game:GetService("Workspace")["Space Dummy"].Torso.CFrame,math.huge,game.Players.LocalPlayer.Character.Torso.voiceline,game:GetService("Workspace")["Space Dummy"].Humanoid,false)
            game:GetService("ReplicatedStorage").Logic.hitbox:InvokeServer(76,nil,game:GetService("Workspace")["Space Dummy"].Torso.CFrame,math.huge,game.Players.LocalPlayer.Character.Torso.voiceline,game:GetService("Workspace")["Space Dummy"].Humanoid,false)
            wait()
        end
    end)
    btnmoneyI.MouseButton1Click:Connect(function()
        btn=btnmoneyI
        touch()
        Enabled = true
        for i,v in next, debug.getregistry() do
            if type(v) == "string" then
                for a,b in next, debug.getupvalues(v) do
                    if string.find(a, "cooled") or string.find(a, "cooled2") or string.find(a, "cooled3") or string.find(a, "cooled4") or string.find(a, "cooled5") or string.find(a, "cooledz") then
                        debug.setupvalue(v, a, true)
                    end
                end
            end
        end
        
        local function Kills()
            while Enabled == true do 
                for i,v in pairs(game.Workspace:GetChildren()) do
                    if v.Name == "Space Dummy" then
                        game:GetService("ReplicatedStorage").Specials.healevent:FireServer(CFrame.new(nil, nil, nil),math.huge,v.Humanoid,game.Players.LocalPlayer.Character.Torso.voiceline,false)
                        game.ReplicatedStorage.Logic.hitbox:InvokeServer(99, game.Players.LocalPlayer.Character.Head, CFrame.new(nil, nil, nil), math.huge, game.Players.LocalPlayer.Character.Torso.voiceline, v.Humanoid, false, false, false)
                        if Enabled == false then break end
                    end
                end
            end
        end
        
        for i = 1, 130 do
            spawn(Kills)
	    wait(0.5)
        end
    end)
    btnFarmWorth.MouseButton1Click:Connect(function()
        btn=btnFarmWorth
        touch()
        Enabled = true
        for i,v in next, debug.getregistry() do
            if type(v) == "string" then
                for a,b in next, debug.getupvalues(v) do
                    if string.find(a, "cooled") or string.find(a, "cooled2") or string.find(a, "cooled3") or string.find(a, "cooled4") or string.find(a, "cooled5") or string.find(a, "cooledz") then
                        debug.setupvalue(v, a, true)
                    end
                end
            end
        end
        
        local function Kills()
            while Enabled == true do 
                for i,v in pairs(game.Workspace:GetChildren()) do
                    if v.Name == "Holy Dummy" then
                        game:GetService("ReplicatedStorage").Specials.healevent:FireServer(CFrame.new(nil, nil, nil),math.huge,v.Humanoid,game.Players.LocalPlayer.Character.Torso.voiceline,false)
                        game.ReplicatedStorage.Logic.hitbox:InvokeServer(99, game.Players.LocalPlayer.Character.Head, CFrame.new(nil, nil, nil), 1000000000000, game.Players.LocalPlayer.Character.Torso.voiceline, v.Humanoid, false, false, false)
                        if Enabled == false then 
                            break 
                        end
                    end
                end
            end
        end
        
        for i = 1, 130 do
            spawn(Kills)
        end
    end)
    btnOpenStandGUI.MouseButton1Click:Connect(function()
        btn=btnOpenStandGUI
        touch()
        local standcheck = game.CoreGui:FindFirstChild("StandsFarm")
        if standcheck then
            game.CoreGui.StandsFarm.StandsGUI:TweenPosition(UDim2.new(0.498945326, 0, 0.545793176, 0))
        else
            loadstring(game:HttpGet("https://pastebin.com/raw/ejeejNkq", true))()	
        end
    end)
    btnfarmitemI.MouseButton1Click:Connect(function()
        btn=btnfarmitemI
        touch();sair(ItalyGUI);entrar(ItensGUIi)
    end)
    --FarmItems(Italy)
    getAjaMaskI.MouseButton1Click:Connect(function()
        btn=getAjaMaskI
        touch();notif("Searching Aja Mask","When spawned teleport it to you",5);itemget("AjaMask")
    end)
    getCorpse.MouseButton1Click:Connect(function()
        btn=getCorpse
        touch();notif("Searching Corpse Part","When spawned teleport it to you",5);itemget("Corpse Part")
    end)
    getReqArrowI.MouseButton1Click:Connect(function()
        btn=getReqArrowI
        touch();notif("Searching Requiem Arrow","When spawned teleport it to you",5);itemget("RequiemArrow")
    end)
    getAjaI.MouseButton1Click:Connect(function()
        btn=getAjaI
        touch();notif("Searching RedAja","When spawned teleport it to you",5);itemget("RedAja")
    end)
    getDiskI.MouseButton1Click:Connect(function()
        btn=getDiskI
        touch();notif("Searching Disk","When spawned auto use it,remember you need kill Diavolo for spawn it",5)
        local item = workspace:WaitForChild("bossdisc")
        if item then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = item.CFrame
            wait(0.5)
            fireclickdetector(item.ClickDetector)
        end
    end)
    getdioboneI.MouseButton1Click:Connect(function()
        btn=getdioboneI
        touch();notif("Searching Bone","When spawned auto use it",5)
        local item = workspace:WaitForChild("DioBone")
        if item then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = item.CFrame
            wait(0.5)
            fireclickdetector(item.ClickDetector)
        end
    end)
    getdiodiaryI.MouseButton1Click:Connect(function()
        btn=getdiodiaryI
        touch();notif("Searching Diary","When spawned auto use it",5)
        local item = workspace:WaitForChild("DioDiary")
        if item then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = item.CFrame
            wait(0.5)
            fireclickdetector(item.ClickDetector)
        end
    end)
    getmoneybagI.MouseButton1Click:Connect(function()
        btn=getmoneybagI
        touch();notif("Searching Money","When spawned auto use it",5)
        local item = workspace:WaitForChild("MoneyBag")
        if item then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = item.CFrame
            wait(0.5)
            fireclickdetector(item.ClickDetector)
        end
    end)
    storeitaly.MouseButton1Click:Connect(function()
        btn=storeitaly
        touch()
        if usestorage==false then
            usestorage=true
            Textcolorstorei.ImageColor3 = Color3.fromRGB(1, 193, 65)
            storemorioh:TweenPosition(UDim2.new(0.501, 0,0, 0),"Out","Linear",0.1,false,nil)
        else
            usestorage=false
            Textcolorstorei.ImageColor3 = Color3.fromRGB(162, 0, 0)
            storemorioh:TweenPosition(UDim2.new(0, 0,0, 0),"Out","Linear",0.1,false,nil)
        end
    end)
    --SpecialGui
    btnTimeStop.MouseButton1Click:Connect(function()
        btn=btnTimeStop
        touch();notif("Anti-TimeStop","Press 'T' to fast use",5)
        game.Workspace.timestopped.Value = false
    end)
    game.Players.LocalPlayer:GetMouse().KeyDown:connect(function(botao)
        if (botao=="t") then
            game.Workspace.timestopped.Value = false
        end
    end)
    btntpitaly.MouseButton1Click:Connect(function()
        btn=btntpitaly
        touch()
        game:GetService("TeleportService"):Teleport(2731332132, game.Players.LocalPlayer)
    end)
    btnstandstorage.MouseButton1Click:Connect(function()
        btn=btnstandstorage
        touch()
        game.Players.LocalPlayer.PlayerGui.standstore.Enabled = true
    end)
    btnkillgui.MouseButton1Click:Connect(function()
        btn=btnkillgui
        touch()
        local killguicheck = game.CoreGui:FindFirstChild("BossKillGui")
        if killguicheck then
            game.CoreGui.BossKillGui.BossKill:TweenPosition(UDim2.new(0.929, 0,0.584, 0))
        else
            loadstring(game:HttpGet("https://pastebin.com/raw/Ns3kSrmB", true))()	
        end
    end)
    btnalert.MouseButton1Click:Connect(function()
        btn=btnalert
        touch()
        loadstring(game:HttpGet("https://pastebin.com/raw/C4GsUGLV", true))()
    end)
    btndupe.MouseButton1Click:Connect(function()
        if #players > 2 then
            notif("Warning","Dupe function,only can be used in Private Servers with max of 2 players on it",5)
        else
            local plr = game.Players.LocalPlayer
            while wait(.001) do
                game.ReplicatedStorage.Specials.emeraldsplash:FireServer(plr.Character.HumanoidRootPart.CFrame, plr.Character.HumanoidRootPart.CFrame, 5, 3.5, plr.Character.Torso.voiceline, false, false)
            end
        end
    end)
    btnstatschanger.MouseButton1Click:Connect(function()
        btn=btnstatschanger
        touch();sair(SpecialGUI);entrar(StatsChanger)
    end)
    btnesp.MouseButton1Click:Connect(function()
        btn=btnesp
        touch()
        loadstring(game:HttpGet("https://pastebin.com/raw/vwbxDc0u", true))()
    end)
    btninvisible.MouseButton1Click:Connect(function()
        btn=btninvisible
        touch()
        if inv==true then
            inv=false
        elseif inv==false then
            inv=true
        end
        game.ReplicatedStorage.Specials.voiddimension:FireServer(inv)
    end)
    btnshop.MouseButton1Click:Connect(function()
        btn=btnshop
        touch()
        loadstring(game:HttpGet("https://pastebin.com/raw/4kPWmS7v", true))() 
    end)
    btnjotaro.MouseButton1Click:Connect(function()
        btn=btnjotaro
        touch()
        loadstring(game:HttpGet("https://pastebin.com/raw/8RFvg6Yb", true))()
    end)
    btnrohan.MouseButton1Click:Connect(function()
        btn=btnrohan
        touch()
        loadstring(game:HttpGet("https://pastebin.com/raw/gQhkpVgV", true))()
    end)
    btnboom.MouseButton1Click:Connect(function()
        btn=btnboom
        touch()
        loadstring(game:HttpGet("https://pastebin.com/raw/yuX0WpPe", true))()
    end)
    btnfusion.MouseButton1Click:Connect(function()
        btn=btnfusion
        touch()
        loadstring(game:HttpGet("https://pastebin.com/raw/Mt1bi2Hh", true))()
    end)
    --StatsChanger
    powerv.Text = game.Players.LocalPlayer.Power.Value
    endurancev.Text = game.Players.LocalPlayer.Endurance.Value
    specialv.Text = game.Players.LocalPlayer.Special.Value
    potencyv.Text = game.Players.LocalPlayer.Potency.Value
    resiliencev.Text = game.Players.LocalPlayer.Resilience.Value
    speedv.Text = game.Players.LocalPlayer.Speed.Value
    powerc.MouseButton1Click:Connect(function()
        btn=powerc
        touch()
        game.Players.LocalPlayer.Power.Value = powerv.Text
    end)
    endurancec.MouseButton1Click:Connect(function()
        btn=endurancec
        touch()
        game.Players.LocalPlayer.Endurance.Value = endurancev.Text
    end)
    specialc.MouseButton1Click:Connect(function()
        btn=specialc
        touch()
        game.Players.LocalPlayer.Special.Value = specialv.Text
    end)
    potencyc.MouseButton1Click:Connect(function()
        btn=potencyc
        touch()
        game.Players.LocalPlayer.Potency.Value = potencyv.Text
    end)
    resiliencec.MouseButton1Click:Connect(function()
        btn=resiliencec
        touch()
        game.Players.LocalPlayer.Resilience.Value = resiliencev.Text
    end)
    speedc.MouseButton1Click:Connect(function()
        btn=speedc
        touch()
        game.Players.LocalPlayer.Speed.Value = speedv.Text
    end)
    while wait() do
        color = Color3.new((math.sin(workspace.DistributedGameTime/2)/2)+0.5, (math.sin(workspace.DistributedGameTime)/2)+0.5, (math.sin(workspace.DistributedGameTime*1.5)/2)+0.5)
        line.BackgroundColor3 = color
    end
