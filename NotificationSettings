import '../auth/auth_util.dart';
import '../backend/backend.dart';
import '../flutter_flow/flutter_flow_theme.dart';
import '../flutter_flow/flutter_flow_util.dart';
import '../flutter_flow/flutter_flow_widgets.dart';
import 'package:flutter/material.dart';
import 'package:flutter_spinkit/flutter_spinkit.dart';
import 'package:google_fonts/google_fonts.dart';

class NotificationsSettingsWidget extends StatefulWidget {
  const NotificationsSettingsWidget({Key? key}) : super(key: key);

  @override
  _NotificationsSettingsWidgetState createState() =>
      _NotificationsSettingsWidgetState();
}

class _NotificationsSettingsWidgetState
    extends State<NotificationsSettingsWidget> {
  bool? switchListTileValue1;
  bool? switchListTileValue2;
  bool? switchListTileValue3;
  final scaffoldKey = GlobalKey<ScaffoldState>();

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      key: scaffoldKey,
      appBar: AppBar(
        backgroundColor: FlutterFlowTheme.of(context).secondaryBackground,
        automaticallyImplyLeading: false,
        leading: InkWell(
          onTap: () async {
            Navigator.pop(context);
          },
          child: Icon(
            Icons.chevron_left_rounded,
            color: FlutterFlowTheme.of(context).grayLight,
            size: 32,
          ),
        ),
        title: Text(
          FFLocalizations.of(context).getText(
            'sc4ff4ce' /* Notifications */,
          ),
          style: FlutterFlowTheme.of(context).title3,
        ),
        actions: [],
        centerTitle: false,
        elevation: 0,
      ),
      backgroundColor: FlutterFlowTheme.of(context).secondaryBackground,
      body: Container(
        width: MediaQuery.of(context).size.width,
        height: MediaQuery.of(context).size.height * 1,
        decoration: BoxDecoration(
          image: DecorationImage(
            fit: BoxFit.fitWidth,
            image: Image.asset(
              'assets/images/login_bg@2x.png',
            ).image,
          ),
        ),
        child: StreamBuilder<UsersRecord>(
          stream: UsersRecord.getDocument(currentUserReference!),
          builder: (context, snapshot) {
            // Customize what your widget looks like when it's loading.
            if (!snapshot.hasData) {
              return Center(
                child: SizedBox(
                  width: 40,
                  height: 40,
                  child: SpinKitPumpingHeart(
                    color: FlutterFlowTheme.of(context).primaryColor,
                    size: 40,
                  ),
                ),
              );
            }
            final columnUsersRecord = snapshot.data!;
            return Column(
              mainAxisSize: MainAxisSize.max,
              children: [
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(20, 0, 20, 0),
                  child: Row(
                    mainAxisSize: MainAxisSize.max,
                    children: [
                      Expanded(
                        child: Text(
                          FFLocalizations.of(context).getText(
                            'r72zvrv5' /* Choose what notifcations you w... */,
                          ),
                          style: FlutterFlowTheme.of(context).bodyText2,
                        ),
                      ),
                    ],
                  ),
                ),
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(0, 12, 0, 0),
                  child: SwitchListTile.adaptive(
                    value: switchListTileValue1 ??= true,
                    onChanged: (newValue) =>
                        setState(() => switchListTileValue1 = newValue),
                    title: Text(
                      FFLocalizations.of(context).getText(
                        'gjygkr0n' /* Push Notifications */,
                      ),
                      style: FlutterFlowTheme.of(context).title3,
                    ),
                    subtitle: Text(
                      FFLocalizations.of(context).getText(
                        '3y3yhxbk' /* Receive Push notifications fro... */,
                      ),
                      style: FlutterFlowTheme.of(context).bodyText2,
                    ),
                    tileColor: FlutterFlowTheme.of(context).secondaryBackground,
                    activeColor: FlutterFlowTheme.of(context).tertiaryColor,
                    activeTrackColor: FlutterFlowTheme.of(context).primaryColor,
                    dense: false,
                    controlAffinity: ListTileControlAffinity.trailing,
                    contentPadding:
                        EdgeInsetsDirectional.fromSTEB(24, 12, 24, 12),
                  ),
                ),
                SwitchListTile.adaptive(
                  value: switchListTileValue2 ??= true,
                  onChanged: (newValue) =>
                      setState(() => switchListTileValue2 = newValue),
                  title: Text(
                    FFLocalizations.of(context).getText(
                      '1ytebj35' /* Email Notifications */,
                    ),
                    style: FlutterFlowTheme.of(context).title3,
                  ),
                  subtitle: Text(
                    FFLocalizations.of(context).getText(
                      '9lvh5nst' /* Receive email notifications fr... */,
                    ),
                    style: FlutterFlowTheme.of(context).bodyText2,
                  ),
                  tileColor: FlutterFlowTheme.of(context).secondaryBackground,
                  activeColor: FlutterFlowTheme.of(context).tertiaryColor,
                  activeTrackColor: FlutterFlowTheme.of(context).primaryColor,
                  dense: false,
                  controlAffinity: ListTileControlAffinity.trailing,
                  contentPadding:
                      EdgeInsetsDirectional.fromSTEB(24, 12, 24, 12),
                ),
                SwitchListTile.adaptive(
                  value: switchListTileValue3 ??= true,
                  onChanged: (newValue) =>
                      setState(() => switchListTileValue3 = newValue),
                  title: Text(
                    FFLocalizations.of(context).getText(
                      '69d2j74u' /* Location Services */,
                    ),
                    style: FlutterFlowTheme.of(context).title3,
                  ),
                  subtitle: Text(
                    FFLocalizations.of(context).getText(
                      '3k8cuv0d' /* Allow us to track your locatio... */,
                    ),
                    style: FlutterFlowTheme.of(context).bodyText2,
                  ),
                  tileColor: FlutterFlowTheme.of(context).secondaryBackground,
                  activeColor: FlutterFlowTheme.of(context).tertiaryColor,
                  activeTrackColor: FlutterFlowTheme.of(context).primaryColor,
                  dense: false,
                  controlAffinity: ListTileControlAffinity.trailing,
                  contentPadding:
                      EdgeInsetsDirectional.fromSTEB(24, 12, 24, 12),
                ),
                Padding(
                  padding: EdgeInsetsDirectional.fromSTEB(0, 24, 0, 0),
                  child: FFButtonWidget(
                    onPressed: () async {
                      Navigator.pop(context);
                    },
                    text: FFLocalizations.of(context).getText(
                      'isgrgbfs' /* Save Changes */,
                    ),
                    options: FFButtonOptions(
                      width: 190,
                      height: 50,
                      color: FlutterFlowTheme.of(context).primaryColor,
                      textStyle:
                          FlutterFlowTheme.of(context).subtitle2.override(
                                fontFamily: 'Lexend',
                                color: FlutterFlowTheme.of(context).textColor,
                              ),
                      elevation: 3,
                      borderSide: BorderSide(
                        color: Colors.transparent,
                        width: 1,
                      ),
                      borderRadius: BorderRadius.circular(30),
                    ),
                  ),
                ),
              ],
            );
          },
        ),
      ),
    );
  }
}
